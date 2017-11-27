# phonegap-md5
Phonegap MD5 checksum plugin for Android and iOS. The plugin reads large files in chunks and build the md5sum incrementally. It can process much larger files then read the complete content in memory and process it in place.

## install
```
cordova  plugin add https://github.com/chenxustu1/cordova-plugin-fastrde-md5.git
```

## usage
``fileEntry`` is a ``org.apache.cordova.file.FileEntry``
```
function win(md5sum){
    console.log("MD5SUM: " + md5sum);
}
function fail(error){
    console.log("Error-Message: " + error);
}
md5chksum.file(fileEntry, win, fail);
```
