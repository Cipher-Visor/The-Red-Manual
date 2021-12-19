# Checking every port with Nmap

If you are stuck in a CTF, haven't managed to gain a foothold, and think you have looked for every possible opening, consider scanning every port. You likely only scanned the most common ones in the beginning out of conveniance. However, if you think you have discovered and investigated every service but could not find any way of getting in, then there could be other services that you'll be able to leverage. Using nmap to scan the target, specify `-p-`. Every port will be scanned.
