# openapi-generator-issue
A sample repository to demonstrate issues with openapi generator

## Instructions:

`npm install`, any node 10+ version
`npm run build:additional` Observe that the generated code (src/api/default.service.ts) is missing any `additionalProperties` from the schema/they are not imported.

### Working example without additional properties:
Run `npm run build` to see the `specWithoutAdditionalProperties.yaml` spec build as expected