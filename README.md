# Super Sparse Checkout

A way to ONLY fetch and checkout a single commit with a sparse working tree.

```
git init <repo>
cd <repo>
git remote add <url>
```

Initializes a repository that tracks the remote.

```
git sparse-checkout set <DIR_1> <DIR_2>
```

Sets up sparse-checkout so we only pull specified directories.

```
git fetch --depth=1 origin <branch>
git checkout FETCH_HEAD
```

Fetch only latest commit from branch and checkout.