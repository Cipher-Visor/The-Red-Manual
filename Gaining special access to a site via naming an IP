# Gaining special access to a site via naming an IP
Many web servers support a feature where, when addressed by a certain domain name, will allow certain access. A site that may have not been accessable by IP or one domain name before may become accessable by another. A challenge in this is trying to guess what the right domain to address it by is.

On Unix systems, this should be doable by editing the `/etc/hosts` file. When editing the file, enter:
```
[TARGET IP ADDRESS]  [ESTIMATED SPECIAL DOMAIN]
```
When you do this, you locally specify a domain to address the given IP by from then on. Any time you interact with the server from your machine, you can address it by the name you gave it. If the server is restricting access to only when it is addressed by a certain domain name and you guessed correctly in your file, you will gain access.

In many CTF platforms, the typical domain format is `[CHALLENGE NAME].[PLATFORM INITIALS]`. In TryHackMe, the initials part in these secret domains tend to be `thm`. In Hack The Box, it tends to be `htb`.
