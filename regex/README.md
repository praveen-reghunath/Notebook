
### Search for `https://` or `http://`

```
/^(http(s{0,1}):\/\/)/gi
```

### Search for specific file extensions exists in the url

```
/^.*\.(jpg|png|gif|html|doc|htm|pdf|jpeg|js|css|webp|svg|mp4|wav|)$/igm
```

matches
```
    http://google.com/something/css/app.6acd2351.css    
    http://google.com/something/js/app.6acd2351.js    
    http://google.com/something/img/background.975ebf08.webp    
    http://google.com/something/6acd2351.mp4
```
Skips
```
https://google.com/tracker
https://google.com/tracker/
http://google.com
http://google.com/true-up
```
