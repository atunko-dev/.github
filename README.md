# atunko-dev org configuration

Settings-as-code for the `atunko-dev` organisation, applied by
[github/safe-settings](https://github.com/github/safe-settings) running in
Actions mode.

`safe-settings/` is the source of truth for repository settings, labels and
rulesets. Change them here, not in the GitHub UI — a hand edit stands only
until the next sync reverts it.

| Path | Owns |
|---|---|
| `safe-settings/settings.yml` | org-wide defaults (deliberately thin) |
| `safe-settings/deployment-settings.yml` | which repos are out of scope |
| `safe-settings/suborgs/product.yml` | repos with CI — settings, labels, rulesets |
| `safe-settings/suborgs/meta.yml` | repos without CI — settings, labels, no rulesets |

Labels are declarative and destructive: a label on a repo but absent from the
config is deleted on the next sync.
