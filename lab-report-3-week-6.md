# Lab Report 3 Week 6
## Streamlining ssh Configuration
Here is screenshot of my `.ssh/config` file, and I edited it with VScode.\
![Config](Config.png)

To login my account, I do not need to type my username and password; instead, I only need one command `ssh ieng6` to login my account. Here is a screenshot of my command:\
![Login](Login.png)

I used `scp` command to copy a markdown file `index.md` to the remote server. Now, I do not need my account name, as shown below:\
![Copy](Copy.png)

## Setup Github Access from ieng6
My public key is called `id_rsa.pub`. It is stored in `cse15l-lab-reports` repository on GitHub and in `.ssh` directory in my user account.\
![GithubKey](GithubKey.png)
![UserAccount](UserAccount.png)

My private key is called `id_rsa`. It is also stored in `.ssh` directory in my user account.\
![UserAccount](UserAccount.png)

On the remote server, I made some changes to `MarkdownParseTest.java`, committed it, and then pushed it to GitHub with `git` commands.
![CommitAndPush](CommitAndPush.png)

Here is a [link](https://github.com/yuy040/markdown-parser/commit/304c92db39700e15cd79eba9b6fbcfb4eb1bf085) for my commit.

## Copy Whole Directories with `scp -r`
I used the command `scp -r . ieng6:markdown-parse` to copy the whole `markdown-parse` directory:
![Dir1](Dir1.png)
![Dir2](Dir2.png)

I logged into the remote server, and then I compiled and ran the file successfully:
![Running](Running.png)

I combined all command in a line, and here is my result:
![Combine1](Combine1.png)
![Combine2](Combine2.png)