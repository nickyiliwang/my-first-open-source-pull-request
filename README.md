This was going to be my first open-source pull request, but unfortunately the owner has archived the repo, but I will still share what I would've done.

#scope
$location = split-array-to-chunks.js , $browser = should be compatible on modern browser, not sure about IE, \$compile= tests all passed, should compile , not really sure that this means.

#Short description
split a Javascript array into chunks with a specified size using a while loop.

#Long description
Instantiate a new array in the function, and the function accepts your raw array that you want to chunk and the size you want to chunk as arguments, using a while loop you want to set the length of the raw array as a condition, meaning if the raw array has 0 items left, the loop exists. Within the while block, we use splice method to split the raw array data into smaller arrays determined by chunk size argument, and push that into the newly created array, with will also be returned as a 2d array containing all the chunked arrays. I used it for pagination and lazy loading once, not sure if best practice.

# [ARCHIVED: READ MORE](https://github.com/eggheadio-github/stack-overflow-copy-paste/issues/257)

# stack-overflow-copy-paste

> A collection of utility JavaScript functions copy/pasted and slightly modified from StackOverflow answers 😀
> (Not intended to be used in actual programs)

[![travis build](https://img.shields.io/travis/eggheadio-github/stack-overflow-copy-paste.svg?style=flat-square)](https://travis-ci.org/eggheadio-github/stack-overflow-copy-paste)
[![codecov coverage](https://img.shields.io/codecov/c/github/eggheadio-github/stack-overflow-copy-paste.svg?style=flat-square)](https://codecov.io/github/eggheadio-github/stack-overflow-copy-paste)
[![version](https://img.shields.io/npm/v/stack-overflow-copy-paste.svg?style=flat-square)](http://npm.im/stack-overflow-copy-paste)
[![downloads](https://img.shields.io/npm/dm/stack-overflow-copy-paste.svg?style=flat-square)](http://npm-stat.com/charts.html?package=stack-overflow-copy-paste&from=2015-08-01)
[![MIT License](https://img.shields.io/npm/l/stack-overflow-copy-paste.svg?style=flat-square)](http://opensource.org/licenses/MIT)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg?style=flat-square)](https://github.com/semantic-release/semantic-release)
[![PRs Welcome](https://img.shields.io/badge/prs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg?style=flat-square)](http://commitizen.github.io/cz-cli/)

This repo is used as the basis for an [Egghead.io](https://egghead.io) series entitled: [How to Contribute to an Open Source Project on GitHub](https://egghead.io/series/how-to-contribute-to-an-open-source-project-on-github)

This repository exists as a resource for people to learn how to contribute to open source in a safe and friendly environment. Feel free to watch the video series and then contribute to this project. See the [contributing guidelines](https://github.com/eggheadio-github/stack-overflow-copy-paste/blob/master/CONTRIBUTING.md).

## Usage

```javascript
import { flatten, snakeToCamel, clone } from "stack-overflow-copy-paste";

flatten([[1, 2], 3]); // [1, 2, 3]
snakeToCamel("snake-case-string"); // 'snakeCaseString'

const testObj = { a: 1, b: 2 };
const copyObj = clone(testObj);
```

## LICENSE

MIT
