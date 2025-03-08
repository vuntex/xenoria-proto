# Xenoria Protobuf Definitions

This repository contains the Protocol Buffers (protobuf) definitions for Xenoria. These .proto files define the structure of gRPC services and messages used for communication between different components of the Xenoria ecosystem.

## 🚀 Features
- **📡 gRPC Service Definitions** – Define remote procedure calls (RPCs) for seamless service communication.
- **📦 Message Structures** – Ensure consistent data exchange across services.
- **🌍 Cross-Language Compatibility** – Use protobufs with multiple programming languages.
- **📥 Precompiled Dependency** – Easily integrate definitions without manual compilation.

---

## 🛠 Usage

### Use as a Dependency (Recommended)
Instead of compiling the `.proto` files manually, you can include them as a dependency:

#### **Maven**

Add the following repository to your `pom.xml`:

```xml
<repository>
  <id>github</id>
  <url>https://maven.pkg.github.com/vuntex/xenoria-proto</url>
</repository>
```

Then, add the dependency:
```xml
<dependency>
  <groupId>de.vuntex.xenoria</groupId>
  <artifactId>xenoria-proto</artifactId>
  <version>1.0.3</version>
</dependency>
```

## 📂 Compile Protobuf Files Manually

If you prefer compiling the .proto files yourself, follow these steps:

**1. Clone the Repository**

```sh
git clone https://github.com/vuntex/xenoria-proto.git
cd xenoria-proto
```

**2. Install the Protobuf Compiler (protoc)**

- Download from: https://github.com/protocolbuffers/protobuf/releases
- Follow the installation instructions for your OS.

**3. Compile the .proto Files**

```sh
protoc --java_out=./generated/java -I=./proto ./proto/**/*.proto
```
