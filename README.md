Pre-commit hook for Stylelint + styled-components / emotion
=============================

This is the Stylelint hook for [pre-commit](https://github.com/pre-commit/pre-commit). This prevents git commits unless the checks pass.

### Using stylelint with pre-commit

- To use this you first need to install pre-commit(see links below).
- Then create a pre-commit config file and also a stylelint config file in the root of your project.
- Run `pre-commit install` from the root of your project

Finally add this to your `.pre-commit-config.yaml`:

```yaml
  - repo: https://github.com/laurens-dg/pre-commit-stylelint
    rev: '0.2.1'
    hooks:
      - id: stylelint
        additional_dependencies:
        - stylelint@13.7.2
        - stylelint-prettier@1.1.2
        - stylelint-config-standard@20.0.0
 ```

 ### Links
 - For pre-commit: see https://github.com/pre-commit/pre-commit

 - For stylelint: see http://stylelint.io/


