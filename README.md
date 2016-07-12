# Case insensitive file system failing git checkout

This repo is an example on how `git checkout` can fail on case-insensitive file systems.

To reproduce:

```bash
git clone git@github.com:oct82/case-insensitivity-git-checkout.git
cd case-insensitivity-git-checkout
git checkout awesome ## Checks out the lowercase awesome
git checkout AWESOME ## Content hasn't changed
git branch ## Incorrect
```
