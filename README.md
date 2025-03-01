# CFN-Lint Buildkite Plugin

A Buildkite plugin to run AWS CloudFormation Linter (cfn-lint) in a Docker container.

## Example

Add the following to your `pipeline.yml`:

```yaml
steps:
  - label: ":cloudformation: Lint CloudFormation"
    plugins:
      - klahnen/cfn-lint#v1.0.0:
          template: template.yaml
```
