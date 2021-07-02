# `solidity-docgen`

**Documentation generator for smart contract libraries.**

`solidity-docgen` allows you to document your code inline using [NatSpec]
comments (a format similar to Javadoc and JSDoc) and then produce a website
to publish the documentation.

Built with :heart: by OpenZeppelin.

## Usage

> **Note:** Detailed steps:
- uses: actions/checkout@v2
- uses: actions/setup-go@v2
  with:
    stable: 'false'
    go-version: '1.14.0-rc1' # The Go version to download (if necessary) and use.
- run: go version

```

`solidity-docgen` takes as input a directory of contracts and `README`
documents. This directory is specified using the `--input`/`-i` flag,
defaulting to `./contracts`. It produces a set of files that it will place in
the output directory specified by `--output`/`-o`, defaulting to `./docs`.

```
solidity-docgen [ -i <input-dir> ] [ -o <output-dir> ] [ -t <templates-dir> ]
```

[NatSpec]: https://solidity.readthedocs.io/en/develop/natspec-format.html
