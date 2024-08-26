# Deletes all deployments given a Pages project name

## How to

### 1. Install dependencies

`bun install`

### 2. Delete all deployments except for the live production deployment (excluding aliased deployments)

```env
# .env

CF_API_TOKEN=xxx 
CF_ACCOUNT_ID=xxx 
CF_PAGES_PROJECT_NAME=xxx

# Delete all deployments except for the live production deployment
# (INCLUDING aliased deployments, eg. my-branch.exampleproj.pages.dev)
# CF_DELETE_ALIASED_DEPLOYMENTS=true 
```

### 3. run `start` script

`bun run start`
