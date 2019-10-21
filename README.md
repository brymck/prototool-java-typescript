prototool-java-typescript
=========================

This repository uses the [`uber/prototool`][prototool-docker] base image, layering on [Java][grpc-java] and [TypeScript][grpc-ts] gRPC plugins for `protoc`.

Usage
-----

Pull the container:

```bash
docker pull brymck/prototool-java-typescript
```

See the `uber/prototool` [Docker documentation][prototool-docker] on how to run the Docker image, and see the [GitHub documentation][prototool] for details on how to organize your project.

If you have your `prototool.yaml` in your project's base directory, a simple Docker command looks like the following:

```bash
docker run -v "$(pwd):/work" brymck/prototool-java-typescript prototool all
```

[prototool-docker]: https://hub.docker.com/r/uber/prototool
[prototool]: https://github.com/uber/prototool
[grpc-java]: https://github.com/grpc/grpc-java
[grpc-ts]: https://github.com/improbable-eng/ts-protoc-gen