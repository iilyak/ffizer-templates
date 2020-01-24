# tiddlywiki-plugin-template

This is a template for tiddlywiki. 

## Supported features

- automatic deployment of a demo site to github pages
- generate list of commands to run to initialize repository

## Usage

```
ffizer apply --source https://github.com/iilyak/ffizer-templates --source-subfolder tiddlywiki-plugin --destination myplugin
```

## Install ffizer

### NixOS

```
nix-shell --command bash -p rustChannels.nightly.rust
cargo install ffizer --force --features cli
```
