# Inspect a Blob

Assuming you have a repo `repo002` already (e.g., from following the directions in the [002-Create-First-Repo.md] quest)

1. `cd repo002`
2. `tree .git`

Don't have the `tree` command?  Ahh, that will be a quest for another day.  Here is what the output of the tree command would look like if you did have `tree`:

```
➜
  repo002 git:(master) tree .git
.git
├── HEAD
├── config
├── description
├── hooks
│   ├── applypatch-msg.sample
│   ├── commit-msg.sample
│   ├── fsmonitor-watchman.sample
│   ├── post-update.sample
│   ├── pre-applypatch.sample
│   ├── pre-commit.sample
│   ├── pre-merge-commit.sample
│   ├── pre-push.sample
│   ├── pre-rebase.sample
│   ├── pre-receive.sample
│   ├── prepare-commit-msg.sample
│   ├── push-to-checkout.sample
│   └── update.sample
├── info
│   └── exclude
├── objects
│   ├── info
│   └── pack
└── refs
    ├── heads
    └── tags

8 directories, 17 files
➜
  repo002 git:(master)
```

What we are interested in is finding a blob ... but there are none!  The entire git database is stored in `.git/objects` and the directory is empty.  There is nothing in the database yet.  So we have to make a blob.

