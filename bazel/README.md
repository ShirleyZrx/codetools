## install bazelisk/bazel on ubuntu

```
wget https://github.com/bazelbuild/bazelisk/releases/v1.20.0/bazelisk-linux-amd64
chmod +x bazelisk-linux-amd64
sudo mv bazelisk-linux-amd64 /usr/local/bin/bazel

echo '\nexport PATH="/usr/local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

which bazel

bazel version
```

## install bazelisk/bazel on MacOS

```
$ cp bazelisk-darwin-amd64 /usr/local/bin/bazel
$ chmod +x /usr/local/bin/bazel
$ which bazel
/usr/local/bin/bazel

$ bazel version
2024/07/18 01:21:47 Downloading https://releases.bazel.build/7.2.1/release/bazel-7.2.1-darwin-x86_64...
Downloading: 65 MB out of 65 MB (100%)
Bazelisk version: v1.20.0
WARNING: Invoking Bazel in batch mode since it is not invoked from within a workspace (below a directory having a WORKSPACE file).
Extracting Bazel installation...
OpenJDK 64-Bit Server VM warning: Options -Xverify:none and -noverify were deprecated in JDK 13 and will likely be removed in a future release.
Build label: 7.2.1
Build target: @@//src/main/java/com/google/devtools/build/lib/bazel:BazelServer
Build time: Tue Jun 25 15:58:07 2024 (1719331087)
Build timestamp: 1719331087
Build timestamp as int: 1719331087
```
