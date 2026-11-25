# lib-noise-handl

Pure-handl implementation of the `noise` ports.

## Layout

```text
src/index.hnl       the implementation
src/index.test.hnl  the .hnl test suite
pkg.hnl             package manifest — modules, deps, description, license
workflows/gate.yaml               bupha entry (handl-gates) → scripts/hnl-gate.sh
```

## Gate

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```

## License

MIT.
