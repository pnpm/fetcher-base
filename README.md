> this package was moved to https://github.com/pnpm/pnpm

# @pnpm/fetcher-base

> Types for pnpm-compatible fetchers

<!--@shields('npm', 'travis')-->
[![npm version](https://img.shields.io/npm/v/@pnpm/fetcher-base.svg)](https://www.npmjs.com/package/@pnpm/fetcher-base) [![Build Status](https://img.shields.io/travis/pnpm/fetcher-base/master.svg)](https://travis-ci.org/pnpm/fetcher-base)
<!--/@-->

## Installation

```sh
npm i -S @pnpm/fetcher-base
```

## Usage

Here's a template for a fetcher using types from `@pnpm/fetcher-base`:

```ts
import {Resolution} from '@pnpm/resolver-base'
import {
  FetchOptions,
  FetchResult,
} from '@pnpm/fetcher-base'

export async function (
  resolution: Resolution,
  targetFolder: string,
  opts: FetchOptions,
): Promise<FetchResult>
  // ...
  return {
    filesIndex,
    tempLocation,
  }
}
```

## License

[MIT](./LICENSE) © [Zoltan Kochan](https://www.kochan.io/)
