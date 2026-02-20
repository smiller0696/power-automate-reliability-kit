# Kit Components

## Lifecycle Template
Scopes:
- SCOPE - TRY - Main Logic
- SCOPE - CATCH - On Error
- SCOPE - FINALLY

## Standard Variables
- hasError (bool)
- runUrl (string)
- errorMessage (string)
- (optional) correlationId (string)
- (optional) stepName (string)

## Logging Sink (Dataverse example)
Table: Power Automate Failures
Columns:
- Date
- Error Message
- Flow Name
- Run URL
