การตัดข้อความภาษาไทยโดยไม่นับสระลอยและวรรณยุกต์

<img src="https://img.shields.io/badge/dynamic/json?label=version&query=version&url=https%3A%2F%2Fraw.githubusercontent.com%2Fporpldev%2Fthai-sentence-cut%2Fmaster%2Fpackage.json" alt="version">
<img src="https://img.shields.io/badge/dynamic/json?label=license&query=license&url=https%3A%2F%2Fraw.githubusercontent.com%2Fporpldev%2Fthai-sentence-cut%2Fmaster%2Fpackage.json" alt="version">


## Installation

This is a [Node.js](https://nodejs.org/en/) module available through the
[npm registry](https://www.npmjs.com/).

```
$ npm install --save thai-sentence-cut
```

## Usage

```
const { lengthOfThaiString, splitThaiStringByLength } = require('../src');

const str = "ประโยคยาวๆ ที่ใช้ทดสอบการตัดคำและการนับความยาวของตัวอักขระโดยไม่สนใจสระและวรรณยุกต์ไทย";

console.log(lengthOfThaiString(s));

// output:
// 76

console.log(splitThaiStringByLength(s,20));

// output:
// [ 'ประโยคยาวๆ ที่ใช้ทดสอบ',
//   'การตัดคำและการนับความ',
//   'ยาวของตัวอักขระโดยไม่',
//   'สนใจสระและวรรณยุกต์ไทย' ]
```

## Depends
- [wordcut](https://www.npmjs.com/package/wordcut)
