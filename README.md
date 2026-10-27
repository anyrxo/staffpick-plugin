# StaffPick

Hire tested remote staff from your AI app. This plugin connects Claude Code, claude.ai and Cowork, Codex or Gemini CLI to StaffPick's MCP server (`https://staffpick.ai/mcp`) and adds a `hire-remote-staff` skill. Describe the role you need: your AI app turns it into a brief, shows tested people with their English, typing and role quiz scores and monthly cost, and asks you before it sends any intro.

## Install

### Claude Code

```
/plugin marketplace add anyrxo/staffpick-plugin
/plugin install staffpick@staffpick
```

Then run `/mcp`, pick `plugin:staffpick:staffpick` and log in. From a shell: `claude plugin install staffpick --marketplace anyrxo/staffpick-plugin`.

### claude.ai and Cowork

Customize, then Plugins, then Add, then Add marketplace, with `anyrxo/staffpick-plugin`.

### Codex

```
codex plugin marketplace add anyrxo/staffpick-plugin
codex plugin add staffpick@staffpick
codex mcp login staffpick
```

### Gemini CLI

```
gemini extensions install https://github.com/anyrxo/staffpick-plugin
```

Then run `/mcp auth staffpick`.

Every app ends the same way: you log in on staffpick.ai with your email code and choose Allow. For ChatGPT, Cursor, VS Code and other apps, see https://staffpick.ai/agents.

## Data

The plugin sends your hiring request and intros to staffpick.ai. Sign-in is StaffPick's own (OAuth 2.1), and the plugin stores nothing. Profiles are anonymised: first name and last initial, country, test scores and rates, never contact details. StaffPick shares contact details by email only after a worker accepts an intro. The AI app never pays or opens a checkout: plans are started on staffpick.ai, by you.

- Privacy: https://staffpick.ai/privacy
- Terms: https://staffpick.ai/terms
- Developers: https://staffpick.ai/developers

## License

MIT, see [LICENSE](LICENSE).
