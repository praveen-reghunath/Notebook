### How to read file size on disk

```
 var stats = fs.lstatSync(file);
 var out = {};
 out.isDir = stats.isDirectory();
 out.size = stats.size;
 console.log(out);
```
