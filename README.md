# NAV Protobuf repository

This repository contains Protobuf specifications shared across NAV systems.

## What is Protobuf?

Protocol buffers, or _Protobuf_, are Google's language-neutral, platform-neutral, extensible mechanism for serializing structured data. Think XML, but smaller, faster, and simpler. You define how you want your data to be structured once, then you can use special generated source code to easily write and read your structured data to and from a variety of data streams and using a variety of languages.

## Generating source code

### Golang

```
mkdir -p output/go
/usr/local/bin/protoc --plugin=~/go/bin/protoc-gen-go --go_out=output/go/ <file.proto>
```

### Java

```
mkdir -p output/java
/usr/local/bin/protoc --java_out=output/java/ <file.proto>
```
