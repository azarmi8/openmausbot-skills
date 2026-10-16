# OpenMausBot Skills — Concrete QC Team

A collection of reusable, domain-oriented skills for assistants and agents supporting concrete quality control, laboratory data, reporting and engineering workflows.

These skills are written as task guidance. They are not a substitute for the applicable standard, a validated calculation engine, an authorized laboratory procedure or human engineering review.

## Skill catalog

| Skill | Purpose |
|---|---|
| [acceptance-criteria-check](acceptance-criteria-check/SKILL.md) | Review whether outputs include explicit and verifiable acceptance criteria |
| [chart-creation](chart-creation/SKILL.md) | Build clear charts with labels, units and a stated purpose |
| [data-cleaning](data-cleaning/SKILL.md) | Identify missing, malformed, duplicated or inconsistent data before analysis |
| [excel-data-extraction](excel-data-extraction/SKILL.md) | Extract and structure values from spreadsheets |
| [excel-report-generation](excel-report-generation/SKILL.md) | Generate consistent Excel reports while preserving provenance |
| [file-management](file-management/SKILL.md) | Apply safe, traceable file operations |
| [powershell-execution](powershell-execution/SKILL.md) | Guide constrained and inspectable PowerShell execution |
| [python-scripting](python-scripting/SKILL.md) | Structure practical Python automation with validation and error handling |
| [quality-audit](quality-audit/SKILL.md) | Review calculations, criteria, standards references and report completeness |
| [statistical-analysis](statistical-analysis/SKILL.md) | Support descriptive statistics and statistical checks |
| [task-decomposition](task-decomposition/SKILL.md) | Break goals into bounded, verifiable tasks |
| [team-coordination](team-coordination/SKILL.md) | Coordinate specialist roles and handoffs |
| [unit-conversion-concrete](unit-conversion-concrete/SKILL.md) | Assist with concrete-strength unit conversion and comparison context |

## Engineering safety rules

- Do not invent missing inputs, standard clauses, limits or acceptance criteria.
- Keep units and specimen types explicit.
- Separate calculations, assumptions, source evidence and recommendations.
- Mark ambiguous or incomplete inputs for review instead of silently completing them.
- Treat AI output as a draft until checked against the governing reference and authorized engineering process.
- Do not present educational values or synthetic examples as measured laboratory data.

## Repository structure

Each skill lives in its own directory and contains a `SKILL.md` file with its metadata and instructions. Read the relevant skill before applying it to a task.

## Status

This is a public skill-library repository. The quality and suitability of any particular skill depend on its current contents and must be validated for the intended engineering context. No skill by itself proves compliance with a concrete standard.

## Related projects

- [BetonBazBot](https://github.com/azarmi8/BetonBazBot)
- [BetonBaz API](https://github.com/azarmi8/betonbaz-api)
- [Cretiq](https://github.com/azarmi8/cretiq) — private project
- [CRETIQ 6044](https://github.com/azarmi8/standard-6044-interactive)
