# bazel-swift-sha256sum-example

This is an example repository for calling an OpenSSL function from Swift. It
part of the [Prototyping Swift code with Bazel and Homebrew](
    https://aige.eu/posts/prototyping-swift-code-with-bazel-homebrew/
) blog post.

## Running the project

```shell
$ bazel run swift/sha256
INFO: Analyzed target //swift/sha256:sha256 (0 packages loaded, 0 targets configured).
INFO: Found 1 target...
Target //swift/sha256:sha256 up-to-date:
  bazel-bin/swift/sha256/sha256
INFO: Elapsed time: 13.112s, Critical Path: 12.28s
INFO: 3 processes: 1 internal, 1 darwin-sandbox, 1 worker.
INFO: Build completed successfully, 3 total actions
INFO: Build completed successfully, 3 total actions
sha256 sum: d5579c46dfcc7f18207013e65b44e4cb4e2c2298f4ac457ba8f82743f31e930b
```
