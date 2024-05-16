# Working with branches
## Add remote branch
> Initial clone was like
> ```
> git clone --depth 1 --branch <branch1>
> ```

```
git remote set-branches --add origin <branch2>
git fetch origin
git checkout <branch2>
```
## Compare specific file in two branches

```
git diff <branch1> <branch2> path/to/file
```
# Working with submodules
## Reset modified submodules
```
git submodule deinit -f .
git submodule update --init --recursive --checkout
```
[Source](https://stackoverflow.com/a/27415757)
