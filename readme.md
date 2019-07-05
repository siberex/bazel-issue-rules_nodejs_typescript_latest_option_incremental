# Overview

Issue: https://github.com/bazelbuild/rules_nodejs/issues/899

Bazel rules_nodejs 0.32.2 ts_library tsc_wrapped uses incompatible with Typescript 3.5.2 options:

```
error TS5074: Option '--incremental' can only be specified using tsconfig, emitting to single file or when option `--tsBuildInfoFile` is specified.
```


# Build and run with Bazel

```bash
bazel run //:bin
```

# Build with TS compiler and run 

```bash
yarn install
yarn start:prod
```
