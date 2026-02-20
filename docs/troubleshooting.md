# Troubleshooting

## Common issue: errorMessage is blank
Some connectors return inconsistent error bodies.
Mitigation:
- capture action outputs in a Compose
- prefer coalesce() across likely error paths

## Common issue: logging action fails
If the logging sink is unavailable, errors may not persist.
Mitigation options:
- add secondary sink (SharePoint list)
- send Teams alert as fallback
