# Mistakes Log

## Mistake 1
- **What happened:** GitHub kept asking for username and password even after SSH setup.
- **Why it happened:** The remote was still using HTTPS instead of SSH.
- **How I fixed it:** I checked the remote URL and switched it to the SSH version.
- **How I will avoid it next time:** I will verify `git remote -v` early whenever authentication behaves unexpectedly.

## Mistake 2
- **What happened:** I saw a warning saying the remote host identification had changed.
- **Why it happened:** The GitHub host key in my known_hosts file did not match the current one.
- **How I fixed it:** I removed the offending old key entry and tested the SSH connection again.
- **How I will avoid it next time:** I will remember that host key issues are separate from password or repo permission issues.