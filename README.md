README
======

This repository provides the required ProtoBuf message definitions for implementing the Axini plugin adapter protocol.

Information on the semantics of the plugin adapter protocol messages can be found in the Effective AML guide available in AMP.

Protocol Buffers
----------------

The messages of the plugin adapter protocol are defined using the language independent [Google Protocol Buffers](https://developers.google.com/protocol-buffers). From these definitions, code can be generated for [various programming languages](https://developers.google.com/protocol-buffers/docs/overview#cross-lang) to serialize the messages.

After installing Protobuf, use the `protoc` command to generate code in various programming language to include in your plugin adapters.

For example, the following command generates Java classes.

```shell
protoc -I=proto/plugin-adapter/api --java_out=src proto/plugin-adapter/api/*.proto
```
