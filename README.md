# zsh on windows

THIS IS OUTDATED, USE THIS INSTEAD: [autistic-tools](https://github.com/soystemd/autistic-tools)

This guide shows you how to install a nice **Cmder** terminal in Windows,
with **cygwin** and **zsh** (the zoomer shell) as the backend, and a **context-menu button**
to open the terminal anywhere, in any folder that you desire.

## how-to

1. Insall cygwin, cmder and zsh as explained in the following article:

[Guide on installing cygwin, cmder and zsh](https://dev.to/zinox9/installing-zsh-on-windows-37em)
(pdf of the webpage is also available in the repo)

2. Clone the repo and copy the `zsh-here` folder to `C:\cygwin64`
3. Put these lines at the top of your .zshrc file:

```bash
    # cd to the path cygwin was launched from
    cd "$(cygpath -u "$(cat "/cygdrive/c/Temp/cygwin-path")" | tr -d $'\r')"
```

4. Install zsh-here.reg
5. Restart pc (or just log-out, or just restart explorer.exe)
