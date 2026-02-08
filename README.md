# Agent Skills

A portfolio-style collection of OpenClaw skills. Each skill lives in its own folder with a dedicated `SKILL.md`, optional reference notes, and scripts. Use this repo as a launchpad for showcasing, testing, and extending agent capabilities.

## What's inside

Each skill folder typically contains:
- `SKILL.md` with purpose, triggers, and usage examples
- `scripts/` with runnable helpers
- `references/` for setup notes and external docs

## Skills in this repository

| Skill | Description | Location |
| --- | --- | --- |
| Academic Research Hub | Search scholarly sources, download papers, extract citations | [academic-research-hub/SKILL.md](academic-research-hub/SKILL.md) |
| Dataset Finder | Discover and download datasets from major repositories | [dataset-finder/SKILL.md](dataset-finder/SKILL.md) |
| Log Analyzer | Parse and summarize logs for errors, patterns, and timelines | [log-analyzer/SKILL.md](log-analyzer/SKILL.md) |
| Proton Bridge Email | Send email via Proton Bridge with age-encrypted creds | [protom-bridge-email/SKILL.md](protom-bridge-email/SKILL.md) |
| QR Code Generator | Generate QR codes for URLs, WiFi, vCards, and more | [qr-code-generator/SKILL.md](qr-code-generator/SKILL.md) |
| Web Search Hub | DuckDuckGo-based web, news, image, and video search | [web-search-hub/SKILL.md](web-search-hub/SKILL.md) |

## Quick start

1. Pick a skill from the table above.
2. Follow the installation section in that skill's `SKILL.md`.
3. Run the example command from the skill's Quick Reference table.

Example (Web Search Hub):

```bash
python web-search-hub/scripts/search.py "climate policy" --type news --time-range w
```

## Repository layout

```
agent-skills/
	academic-research-hub/
		SKILL.md
		references/
		scripts/
	dataset-finder/
		SKILL.md
		references/
		scripts/
	log-analyzer/
		SKILL.md
	protom-bridge-email/
		SKILL.md
		references/
		scripts/
	qr-code-generator/
		SKILL.md
		references/
		scripts/
	web-search-hub/
		SKILL.md
		scripts/
```

## Adding a new skill

1. Create a new folder at the repo root with a short, kebab-case name.
2. Add a `SKILL.md` that documents purpose, triggers, requirements, and examples.
3. Place executable helpers under `scripts/`.
4. Put setup notes or external guidance under `references/`.
5. Update the skills table in this README.

## Notes

- Skills follow the guidelines at https://agentskills.io/.
- Some skills require OpenClawCLI from https://clawhub.ai/.
- Installation guidance is included per skill. Prefer virtual environments when installing Python dependencies.
- Do not commit secrets. If a skill uses credentials, store them outside the repo.

## License

See [LICENSE](LICENSE).

