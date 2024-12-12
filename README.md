labuser@labuser-virtual-machine:~$ git -version
unknown option: -version
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]
labuser@labuser-virtual-machine:~$ Git  --version
Command 'Git' not found, did you mean:
  command 'git' from deb git (1:2.34.1-1ubuntu1.11)
  command 'wit' from deb wit (3.01a-4)
  command 'vit' from deb vit (2.1.0-2)
Try: sudo apt install <deb name>
labuser@labuser-virtual-machine:~$ git  --version
git version 2.34.1
labuser@labuser-virtual-machine:~$ mkdir test1
labuser@labuser-virtual-machine:~$ cd test 1
bash: cd: too many arguments
labuser@labuser-virtual-machine:~$ cd test1
labuser@labuser-virtual-machine:~/test1$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint: 	git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint: 	git branch -m <name>
Initialized empty Git repository in /home/labuser/test1/.git/
labuser@labuser-virtual-machine:~/test1$ git init
Reinitialized existing Git repository in /home/labuser/test1/.git/
labuser@labuser-virtual-machine:~/test1$ echo "test1">test1
labuser@labuser-virtual-machine:~/test1$ cat test1
test1
labuser@labuser-virtual-machine:~/test1$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	test1

nothing added to commit but untracked files present (use "git add" to track)
labuser@labuser-virtual-machine:~/test1$ git add .
labuser@labuser-virtual-machine:~/test1$ git commit
Aborting commit due to empty commit message.
labuser@labuser-virtual-machine:~/test1$ git commit -m "change1"
[master (root-commit) bdf1dd9] change1
 1 file changed, 1 insertion(+)
 create mode 100644 test1
labuser@labuser-virtual-machine:~/test1$ git remote add origin https://github.com/gauravfor/gitpractise1.git
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor 
Password for 'https://gauravfor@github.com': 
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor   
Password for 'https://gauravfor@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 

remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ 
labuser@labuser-virtual-machine:~/test1$ 
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ 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
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: command not found
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
remote: Permission to gauravfor/gitpractise1.git denied to gauravfor.
fatal: unable to access 'https://github.com/gauravfor/gitpractise1.git/': The requested URL returned error: 403
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com':     
Password for 'https://github.com': 
remote: No anonymous write access.
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ git remote add origin https://github.com/gauravfor/gitpractise1.git
error: remote origin already exists.
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/gauravfor/gitpractise1.git'
labuser@labuser-virtual-machine:~/test1$ git pull -u origin main
error: unknown switch `u'
usage: git pull [<options>] [<repository> [<refspec>...]]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --progress            force progress reporting
    --recurse-submodules[=<on-demand>]
                          control for recursive fetching of submodules

Options related to merging
    -r, --rebase[=(false|true|merges|interactive)]
                          incorporate changes by rebasing rather than merging
    -n                    do not show a diffstat at the end of the merge
    --stat                show a diffstat at the end of the merge
    --log[=<n>]           add (at most <n>) entries from shortlog to merge commit message
    --signoff[=...]       add a Signed-off-by trailer
    --squash              create a single commit instead of doing a merge
    --commit              perform a commit if the merge succeeds (default)
    --edit                edit message before committing
    --cleanup <mode>      how to strip spaces and #comments from message
    --ff                  allow fast-forward
    --ff-only             abort if fast-forward is not possible
    --verify              control use of pre-merge-commit and commit-msg hooks
    --verify-signatures   verify that the named commit has a valid GPG signature
    --autostash           automatically stash/stash pop before and after
    -s, --strategy <strategy>
                          merge strategy to use
    -X, --strategy-option <option=value>
                          option for selected merge strategy
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit
    --allow-unrelated-histories
                          allow merging unrelated histories

Options related to fetching
    --all                 fetch from all remotes
    -a, --append          append to .git/FETCH_HEAD instead of overwriting
    --upload-pack <path>  path to upload pack on remote end
    -f, --force           force overwrite of local branch
    -t, --tags            fetch all tags and associated objects
    -p, --prune           prune remote-tracking branches no longer on remote
    -j, --jobs[=<n>]      number of submodules pulled in parallel
    --dry-run             dry run
    -k, --keep            keep downloaded pack
    --depth <depth>       deepen history of shallow clone
    --shallow-since <time>
                          deepen history of shallow repository based on time
    --shallow-exclude <revision>
                          deepen history of shallow clone, excluding rev
    --deepen <n>          deepen history of shallow clone
    --unshallow           convert to a complete repository
    --update-shallow      accept refs that update .git/shallow
    --refmap <refmap>     specify fetch refmap
    -o, --server-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only
    --negotiation-tip <revision>
                          report that we have only objects reachable from this object
    --show-forced-updates
                          check for forced-updates on all updated branches
    --set-upstream        set upstream for git pull/fetch

labuser@labuser-virtual-machine:~/test1$ git pull origin main
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 894 bytes | 894.00 KiB/s, done.
From https://github.com/gauravfor/gitpractise1
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint: 
hint:   git config pull.rebase false  # merge (the default strategy)
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
labuser@labuser-virtual-machine:~/test1$ git fetch origin main
From https://github.com/gauravfor/gitpractise1
 * branch            main       -> FETCH_HEAD
labuser@labuser-virtual-machine:~/test1$ ls -l
total 4
-rw-rw-r-- 1 labuser labuser 6 Dec 12 02:05 test1
labuser@labuser-virtual-machine:~/test1$ cd ..
labuser@labuser-virtual-machine:~$ git fetch origin main
fatal: not a git repository (or any of the parent directories): .git
labuser@labuser-virtual-machine:~$ ls -l
total 52
drwxr-xr-x 2 labuser labuser 4096 Dec 12 02:34 Desktop
drwxr-xr-x 4 labuser labuser 4096 Dec 12 02:34 Documents
drwxr-xr-x 2 labuser labuser 4096 Dec 18  2023 Downloads
-rw-rw-r-- 1 labuser labuser   53 Dec 18  2023 execute.yml
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Music
-rw-rw-r-- 1 labuser labuser   41 Dec 12 02:38 pass
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Pictures
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Public
drwxrwxr-x 2 labuser labuser 4096 Dec 18  2023 repos
drwx------ 6 labuser labuser 4096 Dec 15  2023 snap
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Templates
drwxrwxr-x 3 labuser labuser 4096 Dec 12 02:05 test1
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Videos
labuser@labuser-virtual-machine:~$ cat text1
cat: text1: No such file or directory
labuser@labuser-virtual-machine:~$ cat test1
cat: test1: Is a directory
labuser@labuser-virtual-machine:~$ ls -l
total 52
drwxr-xr-x 2 labuser labuser 4096 Dec 12 02:34 Desktop
drwxr-xr-x 4 labuser labuser 4096 Dec 12 02:34 Documents
drwxr-xr-x 2 labuser labuser 4096 Dec 18  2023 Downloads
-rw-rw-r-- 1 labuser labuser   53 Dec 18  2023 execute.yml
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Music
-rw-rw-r-- 1 labuser labuser   41 Dec 12 02:38 pass
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Pictures
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Public
drwxrwxr-x 2 labuser labuser 4096 Dec 18  2023 repos
drwx------ 6 labuser labuser 4096 Dec 15  2023 snap
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Templates
drwxrwxr-x 3 labuser labuser 4096 Dec 12 02:05 test1
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Videos
labuser@labuser-virtual-machine:~$ vi test.txt
labuser@labuser-virtual-machine:~$ ls -l
total 56
drwxr-xr-x 2 labuser labuser 4096 Dec 12 02:34 Desktop
drwxr-xr-x 4 labuser labuser 4096 Dec 12 02:34 Documents
drwxr-xr-x 2 labuser labuser 4096 Dec 18  2023 Downloads
-rw-rw-r-- 1 labuser labuser   53 Dec 18  2023 execute.yml
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Music
-rw-rw-r-- 1 labuser labuser   41 Dec 12 02:38 pass
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Pictures
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Public
drwxrwxr-x 2 labuser labuser 4096 Dec 18  2023 repos
drwx------ 6 labuser labuser 4096 Dec 15  2023 snap
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Templates
drwxrwxr-x 3 labuser labuser 4096 Dec 12 02:05 test1
-rw-rw-r-- 1 labuser labuser   21 Dec 12 03:54 test.txt
drwxr-xr-x 2 labuser labuser 4096 Sep 12  2023 Videos
labuser@labuser-virtual-machine:~$ cat test.txt
This is a text file.
labuser@labuser-virtual-machine:~$ cd test1/
labuser@labuser-virtual-machine:~/test1$ vi test2.txt
labuser@labuser-virtual-machine:~/test1$ ls -l
total 8
-rw-rw-r-- 1 labuser labuser  6 Dec 12 02:05 test1
-rw-rw-r-- 1 labuser labuser 24 Dec 12 03:56 test2.txt
labuser@labuser-virtual-machine:~/test1$ cat test1
test1
labuser@labuser-virtual-machine:~/test1$ cat test2.txt 
This is a example file.
labuser@labuser-virtual-machine:~/test1$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	test2.txt

nothing added to commit but untracked files present (use "git add" to track)
labuser@labuser-virtual-machine:~/test1$ git add .
labuser@labuser-virtual-machine:~/test1$ git commit -m "This is a message"
[master 723caf3] This is a message
 1 file changed, 1 insertion(+)
 create mode 100644 test2.txt
labuser@labuser-virtual-machine:~/test1$ git remote add origin http://github.com/gauravfor/gitpractise1.git
error: remote origin already exists.
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/gauravfor/gitpractise1.git'
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
remote: Permission to gauravfor/gitpractise1.git denied to gauravfor.
fatal: unable to access 'https://github.com/gauravfor/gitpractise1.git/': The requested URL returned error: 403
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
remote: invalid credentials
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ git remote -v
origin	https://github.com/gauravfor/gitpractise1.git (fetch)
origin	https://github.com/gauravfor/gitpractise1.git (push)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/gauravfor/gitpractise1.git/'
labuser@labuser-virtual-machine:~/test1$ git remote add remoteurl http://github.com/gauravfor/gitpractise1.git
labuser@labuser-virtual-machine:~/test1$ git push remoteurl master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
warning: redirecting to https://github.com/gauravfor/gitpractise1.git/
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (6/6), 497 bytes | 497.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/gauravfor/gitpractise1/pull/new/master
remote: 
To http://github.com/gauravfor/gitpractise1.git
 * [new branch]      master -> master
labuser@labuser-virtual-machine:~/test1$ ls
test1  test2.txt
labuser@labuser-virtual-machine:~/test1$ nano test1
labuser@labuser-virtual-machine:~/test1$ git add .
labuser@labuser-virtual-machine:~/test1$ git commit -m "changes done"
[master 2c8fbda] changes done
 1 file changed, 1 insertion(+), 1 deletion(-)
labuser@labuser-virtual-machine:~/test1$ git push -u origin master
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 284 bytes | 284.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/gauravfor/gitpractise1.git
   723caf3..2c8fbda  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
labuser@labuser-virtual-machine:~/test1$ git branch
* master
labuser@labuser-virtual-machine:~/test1$ git branch devops1
labuser@labuser-virtual-machine:~/test1$ git checkout devops1
Switched to branch 'devops1'
labuser@labuser-virtual-machine:~/test1$ git branch
* devops1
  master
labuser@labuser-virtual-machine:~/test1$ echo "test3">test1
labuser@labuser-virtual-machine:~/test1$ echo "test3">file1
labuser@labuser-virtual-machine:~/test1$ echo "test4">file2
labuser@labuser-virtual-machine:~/test1$ ls -li
total 16
6160418 -rw-rw-r-- 1 labuser labuser  6 Dec 12 04:51 file1
6160419 -rw-rw-r-- 1 labuser labuser  6 Dec 12 04:51 file2
6162014 -rw-rw-r-- 1 labuser labuser  6 Dec 12 04:51 test1
6162049 -rw-rw-r-- 1 labuser labuser 24 Dec 12 03:56 test2.txt
labuser@labuser-virtual-machine:~/test1$ git add .
labuser@labuser-virtual-machine:~/test1$ git commit -m "change 4"
[devops1 70e9147] change 4
 2 files changed, 2 insertions(+)
 create mode 100644 file1
 create mode 100644 file2
labuser@labuser-virtual-machine:~/test1$ git push -u origin devops1
Username for 'https://github.com': gauravfor
Password for 'https://gauravfor@github.com': 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 315 bytes | 315.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'devops1' on GitHub by visiting:
remote:      https://github.com/gauravfor/gitpractise1/pull/new/devops1
remote: 
To https://github.com/gauravfor/gitpractise1.git
 * [new branch]      devops1 -> devops1
Branch 'devops1' set up to track remote branch 'devops1' from 'origin'.
labuser@labuser-virtual-machine:~/test1$ git branch
* devops1
  master
labuser@labuser-virtual-machine:~/test1$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
labuser@labuser-virtual-machine:~/test1$ git merge devops 1
merge: devops - not something we can merge
labuser@labuser-virtual-machine:~/test1$ git merge devops1
Updating 2c8fbda..70e9147
Fast-forward
 file1 | 1 +
 file2 | 1 +
 2 files changed, 2 insertions(+)
 create mode 100644 file1
 create mode 100644 file2
labuser@labuser-virtual-machine:~/test1$ git log -p
commit 70e9147760087f2def8ca94bcc9705fb3c5f509d (HEAD -> master, origin/devops1, devops1)
Author: David Robichaud <david.robichaud@skillsoft.com>
Date:   Thu Dec 12 04:52:14 2024 -0500

    change 4

diff --git a/file1 b/file1
new file mode 100644
index 0000000..df6b0d2
--- /dev/null
+++ b/file1
@@ -0,0 +1 @@
+test3
diff --git a/file2 b/file2
new file mode 100644
index 0000000..df6b0d2
--- /dev/null
+++ b/file1
@@ -0,0 +1 @@
+test3
diff --git a/file2 b/file2
new file mode 100644
commit 70e9147760087f2def8ca94bcc9705fb3c5f509d (HEAD -> master, origin/devops1, devops1)
Author: David Robichaud <david.robichaud@skillsoft.com>
Date:   Thu Dec 12 04:52:14 2024 -0500

    change 4

diff --git a/file1 b/file1
new file mode 100644
index 0000000..df6b0d2
--- /dev/null
+++ b/file1
@@ -0,0 +1 @@
+test3
diff --git a/file2 b/file2
new file mode 100644
index 0000000..d234c5e
--- /dev/null
+++ b/file2
@@ -0,0 +1 @@
+test4

commit 2c8fbda1d7979c50c6f85778cfaa1fd461b26d49 (origin/master)
Author: David Robichaud <david.robichaud@skillsoft.com>
Date:   Thu Dec 12 04:47:24 2024 -0500

    changes done

diff --git a/test1 b/test1
index a5bce3f..df6b0d2 100644
--- a/test1
+++ b/test1
@@ -1 +1 @@
-test1
+test3

commit 723caf3bdce936f27e5d3e6dea8cf82a08537cb3 (remoteurl/master)
Author: David Robichaud <david.robichaud@skillsoft.com>
Date:   Thu Dec 12 03:58:34 2024 -0500

    This is a message

diff --git a/test2.txt b/test2.txt
new file mode 100644
index 0000000..71087af
--- /dev/null
+++ b/test2.txt
@@ -0,0 +1 @@
+This is a example file.
...skipping...


                   SUMMARY OF LESS COMMANDS

      Commands marked with * may be preceded by a number, N.
      Notes in parentheses indicate the behavior if N is given.
      A key preceded by a caret indicates the Ctrl key; thus ^K is ctrl-K.

  h  H                 Display this help.
  q  :q  Q  :Q  ZZ     Exit.
 ---------------------------------------------------------------------------

                           MOVING

  e  ^E  j  ^N  CR  *  Forward  one line   (or N lines).
  y  ^Y  k  ^K  ^P  *  Backward one line   (or N lines).
  f  ^F  ^V  SPACE  *  Forward  one window (or N lines).
  b  ^B  ESC-v      *  Backward one window (or N lines).
  z                 *  Forward  one window (and set window to N).
  w                 *  Backward one window (and set window to N).
  ESC-SPACE         *  Forward  one window, but don't stop at end-of-file.
  d  ^D             *  Forward  one half-window (and set half-window to N).
  u  ^U             *  Backward one half-window (and set half-window to N).
  ESC-)  RightArrow *  Right one half screen width (or N positions).
  ESC-(  LeftArrow  *  Left  one half screen width (or N positions).
  ESC-}  ^RightArrow   Right to last column displayed.
  ESC-{  ^LeftArrow    Left  to first column.
  F                    Forward forever; like "tail -f".
  ESC-F                Like F but stop when search pattern is found.
  r  ^R  ^L            Repaint screen.
  R                    Repaint screen, discarding buffered input.
        ---------------------------------------------------
        Default "window" is the screen height.
        Default "half-window" is half of the screen height.
 ---------------------------------------------------------------------------

                          SEARCHING

  /pattern          *  Search forward for (N-th) matching line.
  ?pattern          *  Search backward for (N-th) matching line.
  n                 *  Repeat previous search (for N-th occurrence).
  N                 *  Repeat previous search in reverse direction.
  ESC-n             *  Repeat previous search, spanning files.
  ESC-N             *  Repeat previous search, reverse dir. & spanning files.
  ESC-u                Undo (toggle) search highlighting.
  ESC-U                Clear search highlighting.
  &pattern          *  Display only matching lines.
        ---------------------------------------------------
HELP -- Press RETURN for more, or q when done...skipping...
commit 70e9147760087f2def8ca94bcc9705fb3c5f509d (HEAD -> master, origin/devops1, devops1)
Author: David Robichaud <david.robichaud@skillsoft.com>
Date:   Thu Dec 12 04:52:14 2024 -0500

    change 4

diff --git a/file1 b/file1
new file mode 100644
index 0000000..df6b0d2
--- /dev/null
+++ b/file1
@@ -0,0 +1 @@
+test3
diff --git a/file2 b/file2
new file mode 100644
index 0000000..d234c5e
--- /dev/null
+++ b/file2
@@ -0,0 +1 @@
+test4

commit 2c8fbda1d7979c50c6f85778cfaa1fd461b26d49 (origin/master)
Author: David Robichaud <david.robichaud@skillsoft.com>
Date:   Thu Dec 12 04:47:24 2024 -0500

    changes done

diff --git a/test1 b/test1
index a5bce3f..df6b0d2 100644
--- a/test1
+++ b/test1
@@ -1 +1 @@
-test1
+test3

commit 723caf3bdce936f27e5d3e6dea8cf82a08537cb3 (remoteurl/master)
Author: David Robichaud <david.robichaud@skillsoft.com>
Date:   Thu Dec 12 03:58:34 2024 -0500

    This is a message

diff --git a/test2.txt b/test2.txt
new file mode 100644
index 0000000..71087af
--- /dev/null
+++ b/test2.txt
@@ -0,0 +1 @@
labuser@labuser-virtual-machine:~/test1$ git log --oneline
70e9147 (HEAD -> master, origin/devops1, devops1) change 4
2c8fbda (origin/master) changes done
723caf3 (remoteurl/master) This is a message
bdf1dd9 change1
labuser@labuser-virtual-machine:~/test1$ git clone http://github.com/gauravfor/gitpractise1.git
Cloning into 'gitpractise1'...
warning: redirecting to https://github.com/gauravfor/gitpractise1.git/
remote: Enumerating objects: 15, done.
remote: Counting objects: 100% (15/15), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 15 (delta 0), reused 12 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (15/15), done.
labuser@labuser-virtual-machine:~/test1$ ls-li
ls-li: command not found
labuser@labuser-virtual-machine:~/test1$ ls -li
total 20
6160419 -rw-rw-r-- 1 labuser labuser    6 Dec 12 04:59 file1
6160429 -rw-rw-r-- 1 labuser labuser    6 Dec 12 04:59 file2
6160413 drwxrwxr-x 3 labuser labuser 4096 Dec 12 05:02 gitpractise1
6162014 -rw-rw-r-- 1 labuser labuser    6 Dec 12 04:51 test1
6162049 -rw-rw-r-- 1 labuser labuser   24 Dec 12 03:56 test2.txt
labuser@labuser-virtual-machine:~/test1$ cd test1
bash: cd: test1: Not a directory
labuser@labuser-virtual-machine:~/test1$ cdtext1
cdtext1: command not found
labuser@labuser-virtual-machine:~/test1$ cd text1
bash: cd: text1: No such file or directory
labuser@labuser-virtual-machine:~/test1$ cd practise1
bash: cd: practise1: No such file or directory
labuser@labuser-virtual-machine:~/test1$ cd gitpractise1
labuser@labuser-virtual-machine:~/test1/gitpractise1$ ls
README.md
labuser@labuser-virtual-machine:~/test1/gitpractise1$ mkdir dev1
labuser@labuser-virtual-machine:~/test1/gitpractise1$ cd dev1
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git pull http://github.com/gauravfor/gitpractise1.git
warning: redirecting to https://github.com/gauravfor/gitpractise1.git/
From http://github.com/gauravfor/gitpractise1
 * branch            HEAD       -> FETCH_HEAD
Already up to date.
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git init .
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint: 	git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint: 	git branch -m <name>
Initialized empty Git repository in /home/labuser/test1/gitpractise1/dev1/.git/
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git remote -v
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git pull http://github.com/gauravfor/gitpractise1.git master
warning: redirecting to https://github.com/gauravfor/gitpractise1.git/
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 9 (delta 0), reused 9 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (9/9), 729 bytes | 729.00 KiB/s, done.
From http://github.com/gauravfor/gitpractise1
 * branch            master     -> FETCH_HEAD
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ branch
Command 'branch' not found, but can be installed with:
sudo apt install rheolef
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git brach
git: 'brach' is not a git command. See 'git --help'.

The most similar command is
	branch
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git branch
* master
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ ls -li
total 8
6160559 -rw-rw-r-- 1 labuser labuser  6 Dec 12 05:06 test1
6160560 -rw-rw-r-- 1 labuser labuser 24 Dec 12 05:06 test2.txt
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git branch m1
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git checkout m1
Switched to branch 'm1'
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ echo "apple1" > fruit
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ ls
fruit  test1  test2.txt
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git checkout master
Switched to branch 'master'
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ ls
fruit  test1  test2.txt
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git checkout m1
Switched to branch 'm1'
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ ls
fruit  test1  test2.txt
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ git rebase master
Current branch m1 is up to date.
labuser@labuser-virtual-machine:~/test1/gitpractise1/dev1$ 
