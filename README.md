# 29780

## Current behavior
Given helmfile.yaml cannot be processed by Renovate, because of relative path in chart section. 
When Renovate runs locally with
```bash
LOG_LEVEL=debug renovate --platform=local --dry-run=true
```
it fails on 
```json
{
  "err": {
    "message": "file-access-violation-error",
    "stack": "Error: file-access-violation-error ..."
    }
}
```

## Expected behavior

Renovate can process helmfile.yaml and "renew" version of "storage" release

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/29780
