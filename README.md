Pre-commit hook for Styleint
=============================

This is the Stylelint hook for [pre-commit](https://github.com/pre-commit/pre-commit). This prevents git commits unless the checks pass.


### Using styleint with pre-commit

- To use this you first need to install pre-commit(see links below).
- Then create a pre-commit config file and also a stylelint config file in the root of your project.
- Run `pre-commit install` from the root of your project

Finally add this to your `.pre-commit-config.yaml`:

```yaml
  - repo: https://github.com/liamdanger/pre-commit-stylelint
    rev: '0.1.0'
    hooks:
      - id: stylelint
        additional_dependencies:
        - stylelint@13.6.1
        - stylelint-processor-styled-components@1.10.0
        - stylelint-config-styled-components@0.1.1
        - stylelint-config-standard@20.0.0
 ```

 ### Links
 - For pre-commit: see https://github.com/pre-commit/pre-commit

 - For stylelint: see http://stylelint.io/


