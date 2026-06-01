#Script updated. Loop added. 

* **How it work:**
  * Try load token from `.env`.
  * If no token, ask for user/PAT.
  * Attempt download `setup.ps1` via GitHub API to verify credentials.
  * If error (wrong credential/bad token), clear `.env` entry and repeat prompt.
  * If success, save token to `.env` and run script.