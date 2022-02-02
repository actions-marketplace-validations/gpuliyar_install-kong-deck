# Install Kong Gateway Deck
Github Action to install Kong Gateway CLI Deck. The Github action can enable CI to deploy the Kong declarative configuration (yml files) to sync with the Kong Gateway using `deck` CLI.

## Inputs

Name | Description | Required
--- | --- | ---
`version` | Deck CLI version to install | `true`

## Example Usage

```
jobs:
  install-deck:
    runs-on: ubuntu-latest
    steps:
    - name: Install Kong Deck CLI
        uses: gpuliyar/install-kong-deck@v1.0.0
        with:
          # Kong Deck CLI Version to install (Mandatory)
          version: 1.0.0
```
