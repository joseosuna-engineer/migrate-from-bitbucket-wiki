# How to migrate from BitBucket to GitHub

*Extract from https://github.com/aiidateam/aiida-core/wiki/How-to-migrate-from-BitBucket-to-GitHub*

Short notes on what we did to migrate from BitBucket to GitHub, mainly not to lose this information.

1. create repo on github (from web interface)
2. move the repository, going through a bare repository in a local folder::

``` git clone --mirror https://bitbucket.org/aiida_team/aiida_core.git
    cd aiida_core.git
    git remote set-url --push origin git@github.com:giovannipizzi/aiida_core_test.git
    git push --mirror
```
3. move issues: This must be done only once, starting from a new repository without issues or pull requests, to keep the numbering. If something goes wrong, then delete the repository and start again from the very beginning.



