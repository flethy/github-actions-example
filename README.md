# Github Actions Example

Developers love to keep the truth in their repositories. This example shows how easy it is to sync workflows within a repository with flethy Cloud.

Define the following environment variables:

- `FLETHY_WORKSPACE_ID`: Your workspace identifier
- `FLETHY_PROJECT_ID`: Your project identifier
- `FLETHY_ACCESS_TOKEN`: Your access token

The command to update a workflow is the following:

```bash
curl -L -X PUT "https://api.flethy.com/v1/w/$FLETHY_WORKSPACE_ID/p/$FLETHY_PROJECT_ID/wf" \
  -H 'Content-Type: application/json' \
  -H 'Accept: application/json' \
  -H "Authorization: Bearer $FLETHY_ACCESS_TOKEN" \
  -d @./workflow.json
```
