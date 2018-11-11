# eosio-dapp-boilerplate
A simple template for quick dapp development in eosio.

## IDE Recommend
vscode

## Directory structure
- eosiolib - EOSIO contracts library
- libc++ - C++ standard library
- contracts - **your contracts directory**
    - hello - code of contract `hello`
        - hello.cpp - cpp source file
        - hello.hpp - cpp header file
        - hello.clauses.md - ricardian_clauses file (not required)
        - hello.contracts.md - ricardian_clauses action file (not required)
- build.sh - script to compile contract with a given dir name

## How to compile contracts
If you want to compile `hello` contract, just run:
```bash
./build.sh hello
```

And then `hello.wasm` and `hello.abi` will be generated in `contracts/hello/`.