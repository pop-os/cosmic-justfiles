# cosmic-justfiles

Shared justfiles used by COSMIC and Pop!_OS projects.

## Import via curl fetch

```just
mod cargo 'cargo.just'

fetch:
    curl -o cargo.just https://raw.githubusercontent.com/pop-os/cosmic-justfiles/master/cargo.just
```

## Import by installed package

```just
mod cargo '/usr/share/cosmic-justfiles/cargo.just'
```

## Call

Just supports calling module recipes with `{{module}}::{{recipe}}` and `{{module}} {{recipe}}`

```just
just cargo vendor
just cargo::build-vendored
```
