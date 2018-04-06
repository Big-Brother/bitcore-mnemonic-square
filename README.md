BIP39 Mnemonics for Bitcore-Square
=======

[![NPM Package](https://img.shields.io/npm/v/bitcore-mnemonic-square.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-mnemonic-square)
[![Build Status](https://img.shields.io/travis/dashpay/bitcore-mnemonic-square.svg?branch=master&style=flat-square)](https://travis-ci.org/dashpay/bitcore-mnemonic-square)
[![Coverage Status](https://img.shields.io/coveralls/dashpay/bitcore-mnemonic-square.svg?style=flat-square)](https://coveralls.io/r/dashpay/bitcore-mnemonic-square)

A module for [bitcore-square](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-square) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install bitcore-mnemonic-square
bower install bitcore-mnemonic-square
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://bitcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('bitcore-mnemonic-square');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://Big-Brother:566e87145f7d24cf2ede7e308370070332b25882@github.com/Big-Brother/bitcore-square/blob/master/CONTRIBUTING.md) on the main bitcore-square repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/bitcore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
