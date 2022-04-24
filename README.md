# Nova ✨🌙

Abstraction for git repositories.

I started this project mainly to keep practicing Go. I was working on a text editor and with <a href="https://github.com/go-git/go-git">go-git</a> on two different projects so I decided to combine the two.

Nova can clone git repositories in-memory and supports a bunch of plumbing and porcelain-ish git commands. I'm planning to slowly bring more and more feature on it.

```bash
# Either
$ go run main.go
# or
$ nova
```

Nova currently supports several commands:

- <b>nova <FILE_NAME></b> - File I/O
- <b>go to <BRANCH_NAME></b> - Creates branch and/or Checkout
- <b>screenshot</b> - Add and Commit (equivalent to git commit -am ...)
- <b>ls</b> - Lists all the files (does not expand subdirectories yet)
- <b>read <FILE_NAME></b> - Displays the content of a file
- <b>status</b> - Displays the status of the worktree (equivalent to git status)
- <b>log</b> - Displays the commits (equivalent to git log)
- <b>branches</b> - Displays the list of branches
- <b>stop</b> - Exits Nova

more will be added.

Nova is able to edit files in memory with its built-in editor and save them on either on its store or on disk. It won't ever do I/O operations on the real directory (unless explicitly told to do so).

Commands:

<img src="https://i.ibb.co/RHvqqSD/Schermata-2022-04-24-alle-16-08-01.png" style="width: 70%" />

- <b>CTRL+Z</b> - Exit
- <b>CTRL+R</b> - Save on disk
- <b>CTRL+S</b> - Save as memory file
