# Workload Identity Fedration

```
steps:
- name: Google Auth
  uses: 'google-github-actions/auth@v0'
  with:
    # credentials_json: '${{ secrets.GCP_AUTH }}'
    workload_identity_provider: '${{ secrets.WIF_PROVIDER }}'
    service_account: '${{ secrets.SA_EMAIL}}' # the SA to impersonate
```
