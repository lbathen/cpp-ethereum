## Ethereum C++ Client.

By Gav Wood, 2014.

          | Linux   | OSX | Windows
----------|---------|-----|--------
develop   | [![Build+Status](http://build.ethdev.com/buildstatusimage?builder=Linux%20C%2B%2B%20develop%20branch)](http://build.ethdev.com/builders/Linux%20C%2B%2B%20develop%20branch/builds/-1) | [![Build+Status](http://build.ethdev.com/buildstatusimage?builder=OSX%20C%2B%2B%20develop%20branch)](http://build.ethdev.com/builders/OSX%20C%2B%2B%20develop%20branch/builds/-1) | [![Build+Status](http://build.ethdev.com/buildstatusimage?builder=Windows%20C%2B%2B%20develop%20branch)](http://build.ethdev.com/builders/Windows%20C%2B%2B%20develop%20branch/builds/-1)
master    | [![Build+Status](http://build.ethdev.com/buildstatusimage?builder=Linux%20C%2B%2B%20master%20branch)](http://build.ethdev.com/builders/Linux%20C%2B%2B%20master%20branch/builds/-1) | [![Build+Status](http://build.ethdev.com/buildstatusimage?builder=OSX%20C%2B%2B%20master%20branch)](http://build.ethdev.com/builders/OSX%20C%2B%2B%20master%20branch/builds/-1) | [![Build+Status](http://build.ethdev.com/buildstatusimage?builder=Windows%20C%2B%2B%20master%20branch)](http://build.ethdev.com/builders/Windows%20C%2B%2B%20master%20branch/builds/-1)
evmjit    | [![Build+Status](http://build.ethdev.com/buildstatusimage?builder=Linux%20C%2B%2B%20develop%20evmjit)](http://build.ethdev.com/builders/Linux%20C%2B%2B%20develop%20evmjit/builds/-1) | [![Build+Status](http://build.ethdev.com/buildstatusimage?builder=OSX%20C%2B%2B%20develop%20evmjit)](http://build.ethdev.com/builders/OSX%20C%2B%2B%20develop%20evmjit/builds/-1) | N/A

[![Stories in Ready](https://badge.waffle.io/ethereum/cpp-ethereum.png?label=ready&title=Ready)](http://waffle.io/ethereum/cpp-ethereum)

Ethereum is based on a design in an original whitepaper by Vitalik Buterin. This implementation is based on the formal specification of a refinement of that idea detailed in the 'yellow paper' by Gavin Wood. Contributors, builders and testers include Alex Leverington (Clang & Mac building, client multiplexing), Tim Hughes (MSVC compilation & Dagger testing), Caktux (ongoing CI), Christoph Jentzsch (tests), Christian Reissweiner (Solidity), Marek Kotewicz (external JS & JSON-RPC), Eric Lombrozo (MinGW32 cross-compilation), Marko Simovic (original CI), and several others.

### Building

See the [Wiki](https://github.com/ethereum/cpp-ethereum/wiki) for build instructions, compatibility information and build tips. 

### Testing

To run the tests, make sure you clone the tests repository from github.com/ethereum to tests as a sibling to cpp-ethereum.

### Yet To Do

See [TODO](https://github.com/ethereum/cpp-ethereum/wiki/TODO)


### License

See [LICENSE](LICENSE)

### Contributing

All development goes in develop branch - please don't submit pull requests to master.

Please read [CodingStandards.txt](CodingStandards.txt) thoroughly before making alterations to the code base. Please do *NOT* use an editor that automatically reformats whitespace away from astylerc or the formatting guidelines as described in [CodingStandards.txt](CodingStandards.txt).

libweb3jsonrpc/abstractwebthreestubserver.h is autogenerated from the jsonrpcstub executable that comes with the libjsonrpc library (json-rpc-cpp project). It shouldn't be maually altered.

```bash
jsonrpcstub spec.json --cpp-server=AbstractWebThreeStubServer
```
