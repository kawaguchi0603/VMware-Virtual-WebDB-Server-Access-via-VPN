### JSON Editの内容

// Example/default ACLs for unrestricted connections.
{
	"tagOwners": {
		"tag:webserver": ["keita.kawaguchi@iii-inc.co.jp"],
	},

	"grants": [
		// Allow all connections.
		{"src": ["*"], "dst": ["*"], "ip": ["*"]},
	],

	// Define users and devices that can use Tailscale SSH.
	"ssh": [
		{
			"action": "accept",
			"src":    ["autogroup:members"],
			"dst":    ["tag:webserver"],
			"users":  ["autogroup:nonroot", "root"],
		},
	],
}
