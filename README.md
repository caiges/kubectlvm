# kubectlvm

A kubectl version manager.

## Installation

```bash
curl -L https://raw.githubusercontent.com/caiges/kubectlvm/master/kubectlvm -o /usr/local/bin/kubectlvm
chmod +x /usr/local/bin/kubectlvm
```

## Usage

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

```bash
ls -lah /usr/local/bin

lrwxrwxrwx  1 root root   42 Jul  9 21:16 kubectl -> /usr/local/kubectl/versions/v1.8.4/kubectl
```
