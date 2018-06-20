# sol2proto

[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
[![Go Report Card](https://goreportcard.com/badge/github.com/getamis/sol2proto)](https://goreportcard.com/report/github.com/getamis/sol2proto)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/getamis/sol2proto)

The Ethereum ABI to gRPC protobuf transpiler

## Installation

```bash
go get github.com/getamis/sol2proto
```

## Usage

```text
Usage of sol2proto:
      --abi stringArray   ABI files generated by solc
  -o, --output string     Output destination, could be 'stdout', 'stderr' or a directory (default "stdout")
      --pkg string        go package name for the generated proto (default "pb")
```

Output to `stdout`

```bash
sol2proto --pkg awesome --abi MyAwesomeContract.abi > my_awesome_contract.proto
```

Output to a directory

```bash
sol2proto --pkg awesome --abi MyAwesomeContract.abi -o .
```

## License

sol2proto is licensed under the GNU Lesser General Public License v3.0, also included in our repository in the LICENSE file.
