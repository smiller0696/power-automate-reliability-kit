# Overview

The Power Automate Reliability Kit is a drop-in pattern for flows that need consistent failure handling.

Instead of each flow implementing logging and cleanup differently, the kit provides:
- a standard lifecycle (Initialize → TRY → CATCH → FINALLY)
- a consistent set of variables (hasError, runUrl, errorMessage, etc.)
- a logging sink example (Dataverse)
- test scenarios to validate behavior

This repo is intentionally lightweight and focuses on reliability primitives.
