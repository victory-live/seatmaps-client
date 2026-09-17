# seatmaps-client

Monorepo for **`@victory-live/seatmaps-client`**, the client-side JavaScript library that renders interactive Ticket Evolution seat maps. Published to npmjs; previously published as `@ticketevolution/seatmaps-client`.

| Where | What |
|---|---|
| [`packages/seatmaps-client/`](packages/seatmaps-client/) | The library. Its [README](packages/seatmaps-client/README.md) is the consumer documentation and is what npm renders. |
| [`examples/`](examples/) | Runnable usage examples (UMD, CommonJS, React, Vite). |
| [`docs/DEVELOPMENT.md`](docs/DEVELOPMENT.md) | Local setup, tooling (pnpm, Turborepo, tsup, Changesets) and the release flow. |

CI and CD (`.github/workflows/ci.yml`, `cd.yml`) are managed by Terraform in `victory-live/github-infra`; do not edit them here. Releases are cut with Changesets: add a changeset with your change, and the "Version Packages" PR publishes on merge.
