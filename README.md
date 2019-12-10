# openapi-generator-issue
A sample repository to demonstrate issues with openapi generator when generating additional properties

## Reproduction Instructions

1. `npm install`, any node 10+ version
1. `npm run build:additional` [Observe that the generated code (src/api/default.service.ts) is missing any imports to `additionalProperties` from the schema/they are not imported as type interfaces.](https://github.com/ltomes/openapi-generator-issue/blob/master/src/api/default.service.ts#L57)

## Expectations
Generated code properly imports interfaces that are required

### Working example without additional properties:
Run `npm run build` to see the `specWithoutAdditionalProperties.yaml` spec build as expected
