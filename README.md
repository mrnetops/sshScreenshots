# sshScreenshots

Capture screenshots from multiple systems.

Particularly useful for collecting auditing information for PCI, SOX or the like.

Some trivial examples

```bash
$ echo "${exampleHost1} ${exampleHost2}" | sshScreenshots -c ls
```

```bash
$ cat hostList.txt | sshScreenshots -c ls
```
