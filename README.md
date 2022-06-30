# Nuitka example using Bazel

Ultimatelly, we want to use `nuitka` as part of our build process.

Bazel will use a controlled, embedded version of python to run Nuitka.

Test it:

```

# optionally update the pip dependencies
bazel run //third_party:requirements.update

bazel run //tools/nuitka -- --onefile  ntest.py
```
