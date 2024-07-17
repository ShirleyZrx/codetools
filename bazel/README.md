## install bazelisk/bazel

```
wget https://github.com/bazelbuild/bazelisk/releases/v1.20.0/bazelisk-linux-amd64
chmod +x bazelisk-linux-amd64
sudo mv bazelisk-linux-amd64 /usr/local/bin/bazel

echo '\nexport PATH="/usr/local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

which bazel

bazel version
```
