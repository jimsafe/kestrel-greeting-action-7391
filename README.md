# Kestrel greeting

A tiny composite action that prints a friendly greeting in your workflow's
job log. It has no dependencies and finishes in well under a second.

## Usage

```yaml
on: push

jobs:
  hello:
    runs-on: ubuntu-latest
    steps:
      - uses: {ACCT_OWNER.login}/kestrel-greeting-action-<run suffix>@v1
        with:
          who-to-greet: Kestrel watchers
```

## Inputs

| Name | Required | Default | Description |
| --- | --- | --- | --- |
| `who-to-greet` | yes | `World` | Who to greet |

## Licence

MIT
