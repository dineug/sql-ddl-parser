# sql-ddl-parser

> Permissive SQL DDL Parser

[![npm version](https://img.shields.io/npm/v/@dineug/sql-ddl-parser.svg?style=flat-square&color=blue)](https://www.npmjs.com/package/@dineug/sql-ddl-parser) [![GitHub](https://img.shields.io/github/license/dineug/sql-ddl-parser?style=flat-square&color=blue)](https://github.com/dineug/sql-ddl-parser/blob/master/LICENSE) [![PRs](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/dineug/sql-ddl-parser/pulls) [![Codecov](https://img.shields.io/codecov/c/gh/dineug/sql-ddl-parser?logo=codecov&style=flat-square)](https://codecov.io/gh/dineug/sql-ddl-parser) [![CI](https://img.shields.io/github/workflow/status/dineug/sql-ddl-parser/CI?label=CI&logo=github&style=flat-square)](https://github.com/dineug/sql-ddl-parser/actions)

## Document

- [Import SQL DDL support syntax](https://github.com/dineug/sql-ddl-parser/blob/master/src/SQL_DDL_Test_Case.md)

## interface

```typescript
export function tokenizer(input: string): Token[];
export function parser(tokens: Token[]): Statement[];
export function DDLParser(input: string): Statement[];
```

| Name      | Type     |
| --------- | -------- |
| tokenizer | Function |
| parser    | Function |
| DDLParser | Function |

## Install

```bash
$ yarn add @dineug/sql-ddl-parser
or
$ npm install @dineug/sql-ddl-parser
```

## Usage

```javascript
import { DDLParser } from "@dineug/sql-ddl-parser";

const statements = DDLParser("sql ddl...");
```

## License

[MIT](https://github.com/dineug/sql-ddl-parser/blob/master/LICENSE)
