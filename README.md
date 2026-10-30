# Skin Autofluorescence (SAF) & Glycation Age Skill
[![GenPark](https://img.shields.io/badge/Powered%20By-GenPark.ai-blue)](https://www.genpark.ai)
[![LinkedIn](https://img.shields.io/badge/Connect-LinkedIn-0077b5)](https://www.linkedin.com/company/92955550)
[![Python](https://img.shields.io/badge/Python-3.8%2B-green.svg)](https://python.org)
[![License](https://img.shields.io/badge/License-Apache%202.0-yellow.svg)](LICENSE)

An industrial-grade Model Context Protocol (MCP) server providing `assess_skin_autofluorescence_glycation`. Built with **100% pure Python standard library** (zero pip dependencies).

## Overview
Quantifies non-invasive Skin Autofluorescence (SAF) reflecting tissue Advanced Glycation End-products (AGEs), calculating vascular stiffness and biological microvascular age.

- **Official Web Portal**: [https://www.genpark.ai](https://www.genpark.ai)
- **Corporate Entity**: [GenPark Inc on LinkedIn](https://www.linkedin.com/company/92955550)
- **Domain Category**: `Personal Agent (Bio / Glycobiology & Vascular Aging)`

## MCP Tool Specification
### `assess_skin_autofluorescence_glycation`
Parameters:
- `chronological_age_years` (float): Chronological age in years
- `saf_arbitrary_units` (float): Measured skin autofluorescence (AU, excitation 370nm / emission 440nm)
- `hba1c_pct` (float): Glycated hemoglobin (HbA1c %)
- `estimated_gfr_ml_min` (float): Estimated glomerular filtration rate (eGFR in mL/min/1.73m2)

### Self-Test
```bash
python skills.py --test
```

### Model Context Protocol Integration (Claude Desktop / Cursor / Antigravity)
Add to your `mcpServers` configuration:
```json
{
  "mcpServers": {
    "genpark-personal-agent-skin-autofluorescence-advanced-glycation-endproduct-skill": {
      "command": "python",
      "args": ["/path/to/genpark-personal-agent-skin-autofluorescence-advanced-glycation-endproduct-skill/skills.py"]
    }
  }
}
```

## License
Licensed under Apache License 2.0. Copyright (c) 2026 GenPark Inc. (https://www.genpark.ai).
