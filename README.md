# stepzen-login

This action logs into the StepZen Server in the specified `domain`, which defaults to `stepzen.net`.

# What's new

Outputs are used instead of environment variables.

# Usage

## Pre-requisites

Node and StepZen CLI must be installed, see [stepzen-dev/stepzen-install action](https://github.com/stepzen-dev/stepzen-install/blob/main/README.md).

## Inputs

- `domain` - StepZen domain (defaults to stepzen.net)
- `account` - StepZen account name
- `adminkey` - Admin key of the StepZen account
- `max_attempts` - Number of retry attempts.
- `retry_wait_seconds` - Time to wait between retries in seconds.
- `timeout_seconds` - Seconds to wait before attempt times out.

## Outputs

- `domain` - StepZen domain
- `account` - StepZen account name
- `apikey` - API key for the account (not the admin key)

## Example

<!-- start usage -->

```yaml
- uses: stepzen-dev/stepzen-login
  with:
    # StepZen Domain
    # Default: 'stepzen.net'
    domain: ""

    # The StepZen Account to use.
    account: ""

    # The adminkey of the specified StepZen Account, likely stored in secrets
    # [Learn more about creating and using encrypted secrets](https://help.github.com/en/actions/automating-your-workflow-with-github-actions/creating-and-using-encrypted-secrets)
    #
    # Required.
    adminkey: ""
```

<!-- end usage -->
