# ffizer-templates

Repository to host my collections of templates to used with [ffizer](https://github.com/ffizer/ffizer).

# Using templates

```
ffizer apply --source https://github.com/iilyak/ffizer-templates --source-subfolder <template_name>  --destination <target_dir>
```

For example to create new tiddlywiki plugin I would run
```
ffizer apply --source https://github.com/iilyak/ffizer-templates --source-subfolder tiddlywiki-plugin  --destination myplugin
```

# Import one template from another one

Add following section to `.ffizer.yaml` file

```
variables:
  - name: gitignore_what
    default_value: rust,git,visualstudiocode
    ask: Create useful .gitignore (via gitignore.io) for

imports:
  - uri: "git@github.com:ffizer/templates_default.git"
    rev: "master"
    subfolder: "gitignore_io"
```