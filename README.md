# `kineticwallet/renovate-configs`

## Description
- A collection of shareable renovate configs.
- Look at the source of each config to see what they do!
- If you found a bug or want to extend the list of configs, simply create an *issue* or a *pull-request*!

## List Of Configs (A-Z)
| **NAME** | **LINK** |
|:---------|:---------|
| `aftman` | `"github>kineticwallet/renovate-configs:aftman"` |
| `foreman` | `"github>kineticwallet/renovate-configs:foreman` |
| `roblox-ts` | `"github>kineticwallet/renovate-configs:roblox-ts"` |
| `rokit` | `"github>kineticwallet/renovate-configs:rokit"` |

## Example
A `renovate.json` config **example** utilizing a few shared configs & more.
```json
{
	"extends": [
		"config:recommended",
		":pinAllExceptPeerDependencies",
		"github>kineticwallet/renovate-configs:rokit",
		"github>kineticwallet/renovate-configs:roblox-ts",
		"npm:unpublishSafe"
	],
	"packageRules": [
		{
			"matchPackageNames": ["@rbxts/types"],
			"automerge": true,
			"minimumReleaseAge": "0 days"
		}
	]
}
```

## Further Information
- This *repository* is licensed under the **MIT** license!
