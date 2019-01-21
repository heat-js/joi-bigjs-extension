# joi-bigjs-extension

Joi extension for Big.js type

[![npm version](https://badge.fury.io/js/joi-bigjs-extension.svg)](http://badge.fury.io/js/joi-bigjs-extension)
[![Dependencies Status](https://david-dm.org/heat-js/joi-bigjs-extension.svg)](https://david-dm.org/heat-js/joi-bigjs-extension)
[![DevDependencies Status](https://david-dm.org/heat-js/joi-bigjs-extension/dev-status.svg)](https://david-dm.org/heat-js/joi-bigjs-extension#info=devDependencies)
[![Known Vulnerabilities](https://snyk.io/test/npm/joi-bigjs-extension/badge.svg)](https://snyk.io/test/npm/joi-bigjs-extension)

## Installation

```yarn add joi-bigjs-extension```

## Usage

### JavaScript

```javascript
const BaseJoi = require('joi');
const {BigNumberExtension} = require('joi-bigjs-extension');
const Joi = BaseJoi.extend(BigNumberExtension);

const schema = Joi.bignumber().positive().integer().min(10).less(100);
```

### Typescript

```typescript
import * as BaseJoi from 'joi';
import {BigNumber} from 'bignumber.js';
import {BigNumberExtension} from 'joi-bigjs-extension';

const Joi = BaseJoi.extend(BigNumberExtension);

const schema = Joi.bignumber().positive().integer().min(10).less(100);
```

## API
See the [API Reference](https://github.com/heat-js/joi-bigjs-extension/blob/v1.1.3/API.md).

## Development

### Install dependencies

```
npm install
```

### Running tests

```
npm test
```

### Release

```
npm run release patch/minor/major
```

## License

MIT
