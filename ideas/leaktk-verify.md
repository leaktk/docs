# leaktk-verify

A tool to verify that credentials are still active.

## Requirements

1. When possible, support using the creds themselves to verify they're active
1. Support using a separate service account for verifying other creds
1. When possible, support verifying the creds are owned by a certain entity first before deactivating them
1. It should accept leaktk-scanner results as its input
2. Its output should be the input + additional special tags to indicate that creds are live and maybe also to link multiple results together to make up the same cred (that is if one pattern finds the username and another pattern finds the password, this should add a tag to link the two together)

## Needs Discovery

* The legal implications of using creds found on the internet (see req #1)

## Resources

* [trufflehog](https://github.com/trufflesecurity/trufflehog) might be a good source of examples for verifying creds.
