# Pre-Market Audit Feed

Two feeds, both written by Perplexity, both read by downstream agents:

## /research/YYYY-MM-DD.json
Written by: Perplexity Workflow A at 7:00 AM CT
Read by: Claude Routine 1 at 7:30 AM CT
Purpose: 10-ticker primary research output
Schema: see schema_research.md

## /audit/YYYY-MM-DD.json
Written by: Perplexity Workflow B at 8:00 AM CT
Read by: Manus market_open.py at 8:30 AM CT
Purpose: Audit of Claude's proposals; vetoes; macro context
Schema: see schema_audit.md
