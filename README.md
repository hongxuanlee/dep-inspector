# dep-inspector
for npm dependencies inspector

[![Build Status](https://travis-ci.org/hongxuanlee/dep-inspector.svg?branch=master)](https://travis-ci.org/hongxuanlee/dep-inspector)
[![Coverage Status](https://coveralls.io/repos/github/hongxuanlee/dep-inspector/badge.svg?branch=master)](https://coveralls.io/github/hongxuanlee/dep-inspector?branch=master)

### usage

#### command use
```
  npm install -g dep-inspector
```

- dep-inspector -i [ignore]

``` 
   cd yourProject
   dep-inspector
   // or..  ignore some modules, split with ,
   dep-inspector -i mocha,istanbul
```

- command display


![](display.png)


### npm require

```
  npm install dep-inspector
```

```
  const inspector = require('dep-inspector');
  const dir = __dirname; // or your specified path
  inspector({
    path: dir
  }).then((result) => {
     // to do...
  });
```




