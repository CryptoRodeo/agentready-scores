# AgentReady Submissions

Centralized repository for AgentReady assessment submissions. Used by the DevLake AgentReady plugin's submissions collector to bulk-onboard repositories.

## Structure

```
submissions/
└── {org}/
    └── {repo}/
        └── assessment-{timestamp}.json
```

## Current Submissions

| Org | Repository | Score | Certification | Assessed |
|-----|-----------|-------|---------------|----------|
| TSD-UI | rhtas-console-ui | 91.9 | Platinum | 2026-05-14 |
| TSD-UI | trustify-ui | 92.0 | Platinum | 2026-05-20 |

## Usage

The DevLake AgentReady plugin reads this repo via the GitHub Trees API. Configure in scope config:

- `submissionsRepo`: GitHub `owner/repo` for this repository
- `submissionsPath`: path prefix (default: `submissions`)
- `submissionsConnectionId`: GitHub connection ID with read access
