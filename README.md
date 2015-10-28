# shell-task
a shell task prgram

# How to run?
`
npm run test
`

# example
``` javascript
new Task('echo "lets go"')
    .set({
        noInterrupt: false
    })
    .exec('wrong cmd')
    .sleep('www')
    .exec('echo haha')
    .sleep(5000)
    .exec('echo \'it went thru!\'')
    .run(function (err, next) {
        if (err && next) {
            console.log('test log:', err);
            next();
        }
    });
```
