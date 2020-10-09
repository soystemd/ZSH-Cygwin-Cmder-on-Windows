# zsh in windows

1. Insall cygwin, cmder and zsh via this guide
 (pdf of the webpage is also in the repo):

[guide on installing cygwin, cmder and zsh](https://dev.to/zinox9/installing-zsh-on-windows-37em)

2. Clone the repo and copy the `zsh-here` folder to `C:\cygwin64`
3. Add this to the top of your .zshrc or .bashrc or whatever:

```bash
    # cd to the path cygwin was launched from
    cd "$(cygpath -u "$(cat "/cygdrive/c/Temp/cygwin-path")" | tr -d $'\r')"
```

4. Install zsh-here.reg
5. Restart pc (or just log-out, or just restart explorer.exe)
