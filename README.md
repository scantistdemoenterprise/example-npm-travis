CoPilot npm/Travis CI Example

Shows a working setup for using CoPilot to analyze the risk of project dependencies

## Travis CI Setup
The `.travis.yml` file has been modified to upload generated dependency data to CoPilot:

```yaml
after_success:
  - bash <(curl -s https://copilot.blackducksoftware.com/ci/travis/scripts/upload)
```
