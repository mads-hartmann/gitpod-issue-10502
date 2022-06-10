# Example code for gitpod-io/gitpod#10502

There are three interesting commits in this repository that shows how something that worked in node:16.15.0-alpine breaks in node:16.15.1-alpine, and finally how to fix it so node:16.15.1-alpine works again. Below is a link to each commit as well as a link to open that specific commit in Gitpod to reproduce that it works (or doesn't, depending on the commit)

1. **Works with node:16.15.0-alpine ([bc56e2c](https://github.com/mads-hartmann/gitpod-issue-10502/commit/bc56e2c472d943a2461a9f2a8b6348060e63bc11), [open in Gitpod](https://gitpod.io/#https://github.com/mads-hartmann/gitpod-issue-10502/commit/bc56e2c472d943a2461a9f2a8b6348060e63bc11
))**  
    When you open a workspace you'll see that the node program runs and the container exits with exit code 0.
2. **Breaks with node:16.15.1-alpine ([7faa84f](https://github.com/mads-hartmann/gitpod-issue-10502/commit/7faa84f8a010cbfe36065211fab5f9e919604299), [open in Gitpod](https://gitpod.io/#https://github.com/mads-hartmann/gitpod-issue-10502/commit/7faa84f8a010cbfe36065211fab5f9e919604299))**  
    When you open a workspace you'll see that the node program doesn't run and that the container exits with error code 243.
3. **Works with node:16.15.1-alpine ([cfc5e77](https://github.com/mads-hartmann/gitpod-issue-10502/commit/cfc5e77fa57f8600383a79a76734824dc17468fe), [open in Gitpod](https://gitpod.io/#https://github.com/mads-hartmann/gitpod-issue-10502/commit/cfc5e77fa57f8600383a79a76734824dc17468fe))**  
    When you open a workspace you'll see that the node program runs and the container exits with exit code 0.

