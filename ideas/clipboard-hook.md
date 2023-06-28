# Clipboard Hook

Monitor clipboard changes and scan clipboard contents, notifying user of secrets.

This could cause heavy loads. Some limitations we could implement:
 - Scanning only when content > 50 characters
 - Only notify when the secret is part of larger contents, this will allow copy/paste of credentials.

