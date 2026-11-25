# lib-noise-handl

Pure-handl implementation of the `noise` ports.

## Layout

| path | role |
| --- | --- |
| `src/index.hnl` | the implementation |
| `src/index.test.hnl` | the .hnl test suite |
| `pkg.hnl` | manifest — `modules: ["noise-handl"]`, dep `noise` |
| `scripts/hnl-gate.sh`, `workflows/gate.yaml` | the gate / bupha entry |

## Contract

- Implements the `noise` contract (`lib-noise`) entirely in handl.

## Verification

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```

## License

MIT.

<!-- myco:agent-awareness -->

## Agent awareness

- Session start / any work discussion: run `myco status --prompt`
  before proposing next steps — know the board first.
- User describes new work → offer to capture it (`myco todo add`,
  `issue new`, `proposal new`). Don't wait to be asked.
- Picking up a task: `myco resume <ID>` is the briefing.
- Wrapping up: `myco handoff <ID>` anything resumable; keep statuses
  honest (claimed → in-progress → blocked/done).

<!-- /myco:agent-awareness -->
