# SlingStrike Community Library

Community-contributed content for [www.slingstrike.com](https://www.slingstrike.com) - use cases, objects, and variables shared under CC-BY-4.0 and distributed for free of charge.

## Structure

- `usecases/` - `.olf` use case files, organized by MITRE ATT&CK tactic and technique (e.g. `TA0006 Credential Access/T1110 Brute Force/`). Each `.olf` file is a single YAML 1.2 document - one file, one use case.
- `objects/` - reusable value lists (usernames, hostnames, IPs, etc.) referenced by use cases.
- `variables/` - reusable generated-value presets referenced by use cases.

## Contributing

Every use case PR must:

- Map to at least one MITRE tactic (`TAxxxx`) and technique (`Txxxx` or `Txxxx.xxx`)
- Use a supported log format: CEF, LEEF, JSON, RFC 3164/5424, WinEvtXML, or Custom
- Avoid hard-coded real IP addresses, hostnames, or credentials
- Include a description of at least 2 sentences explaining the simulated scenario
- Set `olf_version` to the current value published in `docs/spec/olf-format.md` in the main repo
- Come from a contributor who has accepted the project CLA (recorded automatically on PR submission)

Full contribution guidelines, licensing details, and the `.olf` format spec live in the [main repository](https://github.com/slingstrike/slingstrike-community-olf)'s `CONTRIBUTING.md`.

## License

Content in this repository is licensed under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/).
