# Testing

## Test 1: Expression failure (guaranteed)
In TRY scope, add a Compose:
div(1, 0)

Expected:
- TRY fails
- CATCH creates a Dataverse log record
- FINALLY still runs

## Test 2: Invalid Dataverse write (optional)
Temporarily break the Dataverse connection and run again.

Expected:
- Flow fails while attempting to log (document behavior)
- Recommended mitigation: secondary sink (future enhancement)
