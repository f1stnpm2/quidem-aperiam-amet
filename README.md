# [Akili](http://@f1stnpm2/quidem-aperiam-ametjs.com) [![npm version](https://badge.fury.io/js/@f1stnpm2/quidem-aperiam-amet.svg)](https://badge.fury.io/js/@f1stnpm2/quidem-aperiam-amet) [![Build status](https://github.com/f1stnpm2/quidem-aperiam-amet/workflows/build/badge.svg)](https://github.com/f1stnpm2/quidem-aperiam-amet/actions) [![Coverage Status](https://coveralls.io/repos/github/ortexx/@f1stnpm2/quidem-aperiam-amet/badge.svg?branch=master)](https://coveralls.io/github/ortexx/@f1stnpm2/quidem-aperiam-amet?branch=master)

Akili is a component-based javascript framework. 
It includes a powerful system of components, router, store to save and distribute data, functions to make ajax requests and some useful utils.

* very easy for learning, using and testing
* without any additional dependencies
* can be used without javascript compilation in all modern browsers
* pure, lightweight, expandable and powerful framework
* supports [server-side rendering](https://github.com/f1stnpm2/quidem-aperiam-amet-connect)
* javascript way, without magic

## Examples

```js
class HelloWorld extends Akili.Component {
  created() {
    this.scope.count = 0;
    this.scope.title = 'Hello World';
  }
}

Akili.component('hello-world', HelloWorld);

document.addEventListener('DOMContentLoaded', () => {
  Akili.init().catch(err => console.error(err));
});
```

```html
<body>
  <hello-world>
    <div on-click="${ this.count++ }">
      ${ this.title }: ${ this.count }
    </div>
  </hello-world>
</body>
```

More simple examples are on the [site](https://@f1stnpm2/quidem-aperiam-ametjs.com).  
And you can [see the complete example](https://example.@f1stnpm2/quidem-aperiam-ametjs.com) of architecture and [get the source code](https://github.com/f1stnpm2/quidem-aperiam-amet-example).

## Installation
You can install it via npm

```
npm install @f1stnpm2/quidem-aperiam-amet --save
```

or [download](https://@f1stnpm2/quidem-aperiam-ametjs.com/js/libs/@f1stnpm2/quidem-aperiam-amet.js) and include as a script
 
```
<script src="/@f1stnpm2/quidem-aperiam-amet.js"></script>
```

## Documentation
Documentation is [here](https://@f1stnpm2/quidem-aperiam-ametjs.com/docs/getting-started).

## Plugins
* [@f1stnpm2/quidem-aperiam-amet-localization](https://github.com/f1stnpm2/quidem-aperiam-amet-localization)
* [@f1stnpm2/quidem-aperiam-amet-tabs](https://github.com/f1stnpm2/quidem-aperiam-amet-tabs) 

## License
Akili is [MIT licensed](/LICENSE).


 
