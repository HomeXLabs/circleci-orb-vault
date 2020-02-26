# CircleCI Orb for Vault

This orb can be used to retrieve credentials from Vault.

### Supported Credentials:

* AWS IAM User

### Supported Login Methods:

* AppRole

**Note:** You cannot have AWS_ACCESS_KEY_ID and AWS_SECRET_KEY_ID variables set in the project's environment variables since this conflicts with the Orb generating its own credentials.

## Environment variables

These are the environment variables that need to be set within your project:

| Name | Description | Value |
|------|-------------|-------|
| VAULT_ADDR | The address for the vault service | https://vault.homexlabs.com |
| VAULT_ROLE_ID | This specifies the AppRole ID to authenticate to vault | |
| VAULT_SECRET_ID | This is the Secret ID for the AppRole ID | |
