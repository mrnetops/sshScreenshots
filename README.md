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

```
Options:

        -c <command>
                Specify command to run over ssh
        -u <user>
                Specify ssh user
		Default is root
        -o <output>
                Specify output directory
		Default is ./
	-t <timeout>
		Specify per host timeout in seconds
		Default is 120 
        -p <prompt>
                Specify prompt string we are looking for
		Default is ${USER}@
        -d
                Print debugging information
```
