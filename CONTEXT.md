# Alabama ICE Witness - Context for Claude Code

## CRITICAL: READ THE MASTER CONTEXT FIRST

**STOP. Before doing ANYTHING, you MUST read:**

```
us-ice-witness/CONTEXT.md
```

**That file contains ALL the instructions for:**
- How to add incidents
- Incident schema and required fields
- How to process media
- The 5 incident categories
- Validation rules
- Deployment process

**This file only contains Alabama-specific information. The master context has everything else.**

If `us-ice-witness/` doesn't exist, create the symlink first:
```bash
ln -s ../GIT_US_ICE_WITNESS us-ice-witness
```

---

## Alabama State Info

| Field | Value |
|-------|-------|
| State Code | **AL** |
| State Name | Alabama |
| Site URL | al.ice-witness.org |
| Data URL | al-ice-witness.pages.dev |

## Alabama-Specific Context

**Key Communities:**
- Birmingham (largest city, active immigrant advocacy)
- Russellville/Franklin County (poultry workers)
- Gulf Shores/Baldwin County (construction)
- Mobile (Gulf Coast port)

## Alabama News Sources

See `NEWS-SOURCES.md` for state-specific news sources to monitor.

## Quick Reference

**Add an incident:**
```
"Add this incident: [paste news URL]"
```

**Process media:**
```
"I put a video in raw_media for the [incident-slug] incident. Process it."
```

**Generate summary:**
```bash
python3 us-ice-witness/bin/generate_summary.py
```

**Remember: All detailed instructions are in `us-ice-witness/CONTEXT.md`**
