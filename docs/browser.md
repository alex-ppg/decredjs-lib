# Browser

```html
<html>
<head>
<script src="../decredjs-lib.js"></script>
<script>
var Decred = require('decredjs-lib')
var privateKey;
try {
    privateKey = new Decred.PrivateKey('3W3BjaSFmB8e8kXYHGHRJ3TkNksZYfWmnhwSt8XA75E73ZgpRbYxf6', 'dcrdlivenet')
} catch (e) {
    console.error(e)
}
var address = privateKey.toAddress().toString()
var pubKey = privateKey.publicKey.toString()
console.log(pubKey, address)
</script>
</head>
<body>
Hello, Decred
</body>
</html>
```