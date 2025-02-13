# Secrets Analysis

When finding things like ssh keys or other secrets that include metadata
in the secret itself, go ahead and extract that data.

Examples:

- SSH Private Key - comment in the key
- AWS Access Key ID - the AWS account ID
