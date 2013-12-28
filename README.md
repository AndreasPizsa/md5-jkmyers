# md5-jkmyers

Joseph K. Myers' high performance (in fact, the fastest) MD5 implementation for npm, Bower, Component, etc.

[![Endorse on Coderwall](http://api.coderwall.com/andreaspizsa/endorsecount.png)](http://coderwall.com/andreaspizsa)
[![Built with Grunt](https://cdn.gruntjs.com/builtwith.png)](http://gruntjs.com/)

This MD5 implementation was written by [Joseph K. Myers](http://www.myersdaily.org/joseph/javascript/md5-text.html) and is currently the fastest according to [jsperf](http://jsperf.com/md5-shootout). I've wrapped it up as a universal module ([UMD](https://github.com/umdjs/umd)) for easy consumption with [Bower](https://github.com/bower/bower), [Component](https://github.com/component/component), npm, [RequireJS](https://github.com/jrburke/requirejs) ([AMD](https://github.com/amdjs/amdjs-api/wiki/AMD)), [CommonJS](http://wiki.commonjs.org/wiki/CommonJS), etc...


## Usage
The module exports a single function that takes one parameter:
```javascript
md5(String)
```

### On the Client
#### Bower

    bower install md5-jkmyers

#### Component
    component install md5-jkmyers

Then in your `html`, do

```html
 <script type="text/javascript" src="bower_components/md5-jkmyers/md5.min.js"></script>
 <script type="text/javascript">
   console.log(md5('hello, world!'));
 </script>
```

 
### On the Server
#### node.js

Please be aware that node already comes with MD5 built in - see [here](http://stackoverflow.com/a/11869589/199263). Having said that, `md5-jkmyers`  might still be a good and fast alternative (please feel free to contribute perfomance testst):

    npm install md5-jkmyers
    
Then in your code do

    md5 = require('md5')
    md5('hello, world!')

   
## Contributors

- Joseph K. Myers (http://www.myersdaily.org/joseph/) 
- Andreas Pizsa (https://github.com/andreaspizsa)

## Licenses

### Joseph Myers
Joseph Myers does not specify a particular license for his work.

### Andreas Pizsa
MIT

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/AndreasPizsa/md5-jkmyers/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
