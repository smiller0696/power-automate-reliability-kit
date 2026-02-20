# Setup

## 1) Create logging table (Dataverse)
Create a table named (example) "Power Automate Failures" with:
- Date (DateTime)
- Error Message (Multiline Text)
- Flow Name (Text)
- Run URL (Text)

## 2) Create the flow using the kit outline
Follow: /src/template-outline.md

## 3) Add your business logic
Place your actual process inside:
SCOPE - TRY - Main Logic

## 4) Validate it
Run the tests in: /docs/testing.md
