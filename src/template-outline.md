# Template Outline

## Trigger
- Manual trigger (replaceable with any trigger)

## Initialize
- Initialize hasError = false
- Initialize runUrl = <current run URL>
- Initialize errorMessage = ""

## TRY Scope
- Your main business logic goes here
- Optional: isolate retry-prone actions in their own scopes

## CATCH Scope (run after TRY fails)
- Set hasError = true
- Set errorMessage using failed action outputs
- Create Dataverse row in "Power Automate Failures": (can be an email notification or something similar instead of or in addition to the Dataverse row)
  - Date = utcNow()
  - Error Message = errorMessage
  - Flow Name = workflow()?['name']
  - Run URL = runUrl

## FINALLY Scope (always runs)
- Cleanup actions
- Optional: success telemetry, notifications, etc.
