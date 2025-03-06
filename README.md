# Xenoria Protobuf Definitions

This repository contains the Protocol Buffers (protobuf) definitions for Xenoria. These .proto files define the structure of gRPC services and messages used for communication between different components of the Xenoria ecosystem.

## 🚀 Features
- **gRPC Service Definitions** – Define remote procedure calls (RPCs) for seamless service communication.
- **Message Structures** – Ensure consistent data exchange across services.
- **Cross-Language Compatibility** – Use protobufs with multiple programming languages.

## 🛠 Usage
### Clone the Repository
```sh
git clone https://github.com/your-username/xenoria-protobuf.git
cd xenoria-protobuf
```

## 📂 Compile Protobuf Files

Ensure you have the Protobuf compiler installed (protoc).
Generate code for your desired language (e.g., Java, Python, TypeScript):

```sh
protoc --java_out=./generated/java -I=./proto ./proto/**/*.proto
```
