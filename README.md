# Deletes all deployments given a Pages project name

## How to

### Install dependencies
`bun install`

### Delete all deployments except for the live production deployment (excluding aliased deployments)
`.env`
```
CF_API_TOKEN=xxx 
CF_ACCOUNT_ID=xxx 
CF_PAGES_PROJECT_NAME=xxx 
```
and then,
```bun run start```

### Delete all deployments except for the live production deployment (INCLUDING aliased deployments, eg. my-branch.exampleproj.pages.dev)
`.env`
```
CF_API_TOKEN=xxx 
CF_ACCOUNT_ID=xxx 
CF_PAGES_PROJECT_NAME=xxx 
CF_DELETE_ALIASED_DEPLOYMENTS=true 
```
and then,
`bun run start`
