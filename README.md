# memory
this is a collection of different things that I've found useful and need to jump back to sometimes

----------

 - **qr code generator**

```
http://chart.googleapis.com/chart?chs=200x200&cht=qr&chl=http://www.google.com
```

- **zero disc space**

```
cat /dev/zero > zero.fill; sync; sleep 1; sync; rm -f zero.fill
```

- **tar form svn working copy (exclude .svn dirs)**

```
tar --exclude=\.svn
```

- **change file extensions (with files with space....don't forget to escape spaces)**

```
for f in *.htm; do mv $f `basename $f .htm`.html; done;
```

- **maven command for building APK**

```
mvn clean package -Dandroid.sdk.path=<path to android sdk>
```

- **cmis workbench oauth**

```
org.apache.chemistry.opencmis.binding.atompub.url=https://api.alfresco.com/cmis/versions/1.1/atom
org.apache.chemistry.opencmis.binding.auth.http.basic=false
org.apache.chemistry.opencmis.binding.header.0=Authorization:Bearer f526e412-f5bc-44a0-879e-9a210e510be3
org.apache.chemistry.opencmis.binding.compression=true 
cmis.workbench.folder.includeAcls=false 
cmis.workbench.object.includeAcls=false 
cmis.workbench.version.includeAcls=false
```

