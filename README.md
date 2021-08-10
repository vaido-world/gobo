# Gobo-Linux-Information

`curl https://vaido.world/Gobo-Linux-Information/vbox.bash | bash`

**https://github.com/gobolinux/Documentation/wiki/Running-under-VirtualBox**

http://download.virtualbox.org/virtualbox/5.2.44/

## xfce
https://github.com/gobolinux/Recipes/issues/136#issuecomment-892838195


## Search for DocBook

`grep -rnw '/' -e 'DocBook'`


https://github.com/gobolinux/Recipes/issues/136#issuecomment-892838195



`find / catalog`

```
find / catalog -not -path "/System/Kernel/*"  -not -path "/Programs/Python*" -not -path "/Programs/OpenSSL*"
```


```
find / -name "catalog"
/Data/Variable/lib/xml/catalog
/Data/Variable/run/rootfsbase/Data/Variable/lib/xml/catalog

```

```
nano /Data/Variable/lib/xml/catalog
```

```
root@LiveCD ~]     
find / -name "catalog.xml"
/Data/Variable/run/rootfsbase/Programs/DocBook-XSL-Stylesheets/1.79.1/share/xml/docbook/stylesheet/docbook-xsl/catalog.xml
/Programs/DocBook-XSL-Stylesheets/1.79.1/share/xml/docbook/stylesheet/docbook-xsl/catalog.xml

```

### Example
```
file:///Users/root/Desktop/file.txt
```

### Finished

#### This resolves only `could not find DocBook XSL Stylesheets in XML catalog`

```
<nextCatalog catalog="file:///Programs/DocBook-XSL-Stylesheets/1.79.1/share/xml/docbook/stylesheet/docbook-xsl/catalog.xml"/>
```


### Google Search Query

```
gtk-doc DocBook catalog.xml configure: error: could not find DocBook XML DTD V4.3 in XML catalog
```


Worth A try: https://trac.macports.org/ticket/17662

try to `nano /Data/Variable/run/rootfsbase/Data/Variable/lib/xml/catalog`

### New Google Query

`gtk-doc could not find DocBook XML DTD  in XML catalog -Stylesheets`

https://trac.macports.org/ticket/17560

https://lists.macports.org/pipermail/macports-tickets/2009-September/039793.html

## Removing locally the whole gtk-doc from configure script
https://mail.gnome.org/archives/gtk-osx-users-list/2015-January/msg00000.html


## `/opt` equals `/Programs`?
https://unix.stackexchange.com/questions/210770/which-linux-distribution-places-all-applications-in-opt/215734#215734


https://github.com/vaido-world/Gobo-Linux-Information/blob/0849f65ab180fa0e12c5a78935ac6624d1682a2b/config.log#L413


```
checking for pkg-config... /usr/bin/pkg-config
checking pkg-config is at least version 0.19... yes
checking for a Python interpreter with version >= 3.2... python3
checking for python3... /usr/bin/python3
checking for python3 version... 3.8
checking for python3 platform... linux
checking for python3 script directory... ${prefix}/lib/python3.8/site-packages
checking for python3 extension module directory... ${exec_prefix}/lib/python3.8/site-packages
checking for xsltproc... /usr/bin/xsltproc
checking for dblatex... no
checking for fop... no
configure: WARNING: neither dblatex nor fop found, so no pdf output from xml
checking for XML catalog... /Data/Variable/lib/xml/catalog
checking for xmlcatalog... /usr/bin/xmlcatalog
checking for DocBook XML DTD V4.3 in XML catalog... not found
configure: error: could not find DocBook XML DTD V4.3 in XML catalog
PrepareProgram: configure failed.
Compile: GTK-Doc 1.33.0 - Configuration failed.
```

https://raw.githubusercontent.com/gobolinux/Recipes/master/Git/2.29.2/Recipe
