If the .runsh/config.yaml file doesn't exist,
create it with the following content:

``` yaml
default_shell: bash
scripts_dir: https://github.com/crimson206/my-scripts/tree/main/scripts/temp
```

After that, you can learn how to perform merge and version tagging simultaneously by running:

``` bash
runsh merge_and_tag -h
```

Use git status to check the current branch, and if it's dev, proceed with merge_and_tag.
If it's a different branch, consult with the user again. 