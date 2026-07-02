# Audit Perspectives

A STORM-style, multi-stakeholder method for audit questions — built as a [Claude Code](https://claude.com/product/claude-code) skill.

Runs any audit question through every layer of an engagement team (Staff through Partner, Core Audit through IT/Tax/Advisory) plus external stakeholders (PCAOB, AICPA, regulators, investors), then maps where the views conflict and synthesizes a practical recommendation.

- **Site:** https://gitmaster-max.github.io/audit-perspectives
- **Skill definition:** [`SKILL.md`](./SKILL.md)

## Install

```bash
mkdir -p ~/.claude/skills/audit-perspectives
curl -o ~/.claude/skills/audit-perspectives/SKILL.md \
  https://raw.githubusercontent.com/gitmaster-max/audit-perspectives/main/SKILL.md
```

Then, inside Claude Code:

```
/audit-perspectives "How should we approach the risk assessment for IBNR reserves at a health insurer?"
```

## Provenance

Adapts Stanford OVAL Lab's STORM method (Shao et al., NAACL 2024) — multi-perspective question asking as a research technique — into an audit-specific framework. Segment structure and hierarchy gradient are original.
