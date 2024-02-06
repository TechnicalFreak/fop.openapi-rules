# Demo-Github-Action

´´´yaml
name: OpenApi Checks

on:
  pull_request:
    branches:
      - master

jobs:
  check:
    uses: TechnicalFreak/fop.openapi-rules/.github/workflows/check-openapi.yaml@1
    with:
      openapi-file-path: my-api.yaml
´´´
