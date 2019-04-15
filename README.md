# dart-arm
Dockerfiles &amp; Docker images for running Dart on Docker

---

# Overview
Official Dart for ARM platforms aren't yet available. Fortunatley offical builds of Dart are available for ARM at [https://www.dartlang.org/tools/sdk/archive](https://www.dartlang.org/tools/sdk/archive). These Dockerfiles define a multi-stage builds for `armv7` and `arm64` targets.

# Usage
Pre-built images are available at [isaacp/dart-arm]https://hub.docker.com/r/isaacp/dart-arm) using either `:armv7` or `:arm64` tags

### Example
Use these in a Dockerfile:
```
FROM isaacp/dart-arm:armv7

...

CMD ["/usr/lib/dart/bin/dart", "/app/main.dart"]
```

# Future
The images on Docker Hub are manually built, but automating is planned. The biggest hurdle is setting up CI/CD on a native (or emulated) ARM environment. Any suggestions/comments welcome!

