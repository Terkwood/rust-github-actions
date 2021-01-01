# how to use github actions to release a rust DLL for windows

Take a look at [the github actions config](./.github/workflows/rust.yml).

After you make some changes that you want published, you need to push
tags to your repo:

```sh
git tag -a v0.0.0-a -m "whatever"
git push --tags
```

Here are the github actions that we rely on for this configuration:

- [rust-toolchain action](https://github.com/actions-rs/toolchain)
- [softprops gh-action-release](https://github.com/softprops/action-gh-release)
