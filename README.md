# kubectlvm

A kubectl version manager.

Install a specific version of kubectl:

```bash
kubectlvm 1.8.4
```

That version is installed under `/usr/local/kubectl`:

```
/usr/local/kubectl/
└── versions
    └── v1.8.4
        └── kubectl
```

A symlink is created pointing to the requested version:

```
ls -lah /usr/local/bin

lrwxrwxrwx  1 root root   42 Jul  9 21:16 kubectl -> /usr/local/kubectl/versions/v1.8.4/kubectl
```
