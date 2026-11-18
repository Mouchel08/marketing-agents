# Marketing Agents

A static dashboard for seven marketing roles: SEO, conversion optimisation, content, paid media, growth, sales and strategy.

## Open the dashboard

Open [dashboard/index.html](dashboard/index.html) in a browser, or use the [GitHub Pages URL](https://mouchel08.github.io/marketing-agents/dashboard/) if Pages is enabled for this repository.

You can search roles and skills, set a role's status, copy a suggested command, or open a new Claude conversation. Status and last-used timestamps are stored in your browser's local storage; they are manually maintained rather than live agent activity.

The Chat button currently opens Claude with the greeting "Hi". It does not load the role's instructions or listed skills. Copying a command such as `/marketing:seo` copies text only; this repository does not supply an implementation of those slash commands.

## Repository contents

- [dashboard/index.html](dashboard/index.html): the dashboard.
- [7 In 1](7%20In%201): an alternative HTML dashboard.
- [LICENSE](LICENSE): MIT licence.

There are currently no `agents/`, `commands/` or `skills/` directories, or Claude Code plugin metadata. Cloning this repository does not install a Claude Code plugin.

## Marketing skills

The dashboard lists skill names by role. The separate [marketingskills repository](https://github.com/Mouchel08/marketingskills) contains marketing skill documents and its own installation instructions.

## Contributing

Changes to this dashboard belong in `dashboard/index.html`. Open that file in a browser and check search, status filters, command copying and Chat links after making a change.

## Licence

[MIT](LICENSE).
