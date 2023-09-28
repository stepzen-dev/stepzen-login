# stepzen-login
This action logs into the StepZen Server in the specified `domain`, which defaults to `stepzen.net`. 

It sets the `STEPZEN_ACCOUNT`, `STEPZEN_APIKEY` and `STEPZEN_DOMAIN` environment variables.

# What's new
First iteration.

# Usage

<!-- start usage -->
```yaml
- uses: stepzen-dev/stepzen-login
  with: 
    # StepZen Domain
    # Default: 'stepzen.net'
    domain: ''

    # The StepZen Account to use.
    account: ''

    # The adminkey of the specified StepZen Account, likely stored in secrets
    # [Learn more about creating and using encrypted secrets](https://help.github.com/en/actions/automating-your-workflow-with-github-actions/creating-and-using-encrypted-secrets)
    #
    # Required. 
    adminkey: ''
```
<!-- end usage -->

