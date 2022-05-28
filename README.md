# Resume Atlas

This Github Action allows you to resume a MongoDB Atlas Cluster. Makes use of [AtlasCLI](https://github.com/jdrumgoole/atlascli)

## How to use this Action

In order to use this action in your workflow, you just need to provide this four settings:
```yaml
steps:
  - name: Resume
    uses: xacobecm/atlas-resume@v1.0
    id: pause-atlas
    with:
      public_api_key: 'public'
      private_api_key: 'private'
      project_id: 'project'
      cluster_name: 'cluster'

```
It is recommended that you store this credentials in [GitHub Secrets](https://docs.github.com/es/actions/security-guides/encrypted-secrets).
