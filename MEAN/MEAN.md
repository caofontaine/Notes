# MEAN

## Passing Client-Side Parameters To Server-Side
[How to pass client-side parameters to the server-side in Angular/Node.js/Express](https://stackoverflow.com/questions/33108326/how-to-pass-client-side-parameters-to-the-server-side-in-angular-node-js-express)

#### Client (GET)
```
   $http.get('/login', {params: {name: 'ABCXYZ'}})
    .success(
        function(success){
            console.log(success)
        })
    .error(
        function(error){
            console.log(error)
        });
```

#### Server (GET)
```
   router.get('/login', function(req, res, next) {
    var username = req.query.name;
    res.json({'status': 200, 'msg': 'success'});
   }
```