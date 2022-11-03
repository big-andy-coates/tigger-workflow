# Trigger workflow

A hack space for trying to get one Github workflow to push tags to git, triggering a second workflow.

As covered in the [Github docs](https://docs.github.com/en/actions/using-workflows/triggering-a-workflow#triggering-a-workflow-from-a-workflow),
if a PAT (personal access token) is used, then it _should_ work...  

Manually running

```shell
git pull
git tag v0.0.<next verion>
git push -tag
```

Does trigger the `Tag Listener`.  Running the `Tag Publisher` workflow does not :(

