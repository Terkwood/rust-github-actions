# demonstrate using github actions to release a dynamic lib

This is useful for building a dynamically-linked lib used by
Godot Engine, e.g. in [delta-pack](https://github.com/Terkwood/delta-pack).

Shows configuration for win, mac, linux x86_64.

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
