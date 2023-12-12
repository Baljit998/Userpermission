frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git reset --hard
HEAD is now at a08a1b9 Removed website_redirects
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git branch
* main
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git remote -v
upstream	https://github.com/Baljit998/F-Drive.git (fetch)
upstream	https://github.com/Baljit998/F-Drive.git (push)
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git pull
remote: Enumerating objects: 7602, done.
remote: Counting objects: 100% (7602/7602), done.
remote: Compressing objects: 100% (1803/1803), done.
remote: Total 7425 (delta 5849), reused 6817 (delta 5583), pack-reused 0
Receiving objects: 100% (7425/7425), 6.55 MiB | 4.03 MiB/s, done.
Resolving deltas: 100% (5849/5849), completed with 127 local objects.
From https://github.com/Baljit998/F-Drive
 + a08a1b9...56b9745 main       -> upstream/main  (forced update)
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
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git stats
git: 'stats' is not a git command. See 'git --help'.

The most similar command is
	status
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git status
On branch main
Your branch and 'upstream/main' have diverged,
and have 1 and 974 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

nothing to commit, working tree clean
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git pull
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
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git pull --rebase
Successfully rebased and updated refs/heads/main.
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git pull
Already up to date.
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git satus
git: 'satus' is not a git command. See 'git --help'.

The most similar command is
	status
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git status
On branch main
Your branch is up to date with 'upstream/main'.

nothing to commit, working tree clean
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ 

frappe@baljit-ThinkPad-T460:~/frappe-bench$ cd apps/
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps$ cd drive/
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git status
On branch mydev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   drive/hooks.py

frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git commit -m "rm redirects"
frontend/.husky/pre-commit: 4: black: not found
husky - pre-commit hook exited with code 127 (error)
husky - command not found in PATH=/usr/lib/git-core:/home/frappe/.nvm/versions/node/v16.20.2/bin:/home/frappe/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/snap/bin
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git branch
  main
* mydev
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ pip install black
Defaulting to user installation because normal site-packages is not writeable
Collecting black
  Downloading black-23.12.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (1.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.7/1.7 MB 2.0 MB/s eta 0:00:00
Requirement already satisfied: platformdirs>=2 in /usr/lib/python3/dist-packages (from black) (2.5.1)
Collecting typing-extensions>=4.0.1
  Downloading typing_extensions-4.9.0-py3-none-any.whl (32 kB)
Requirement already satisfied: tomli>=1.1.0 in /usr/local/lib/python3.10/dist-packages (from black) (2.0.1)
Collecting pathspec>=0.9.0
  Downloading pathspec-0.12.1-py3-none-any.whl (31 kB)
Requirement already satisfied: click>=8.0.0 in /usr/lib/python3/dist-packages (from black) (8.0.3)
Collecting mypy-extensions>=0.4.3
  Using cached mypy_extensions-1.0.0-py3-none-any.whl (4.7 kB)
Requirement already satisfied: packaging>=22.0 in /usr/local/lib/python3.10/dist-packages (from black) (23.1)
Collecting aiohttp>=3.7.4
  Downloading aiohttp-3.9.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (1.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.2/1.2 MB 1.4 MB/s eta 0:00:00
Collecting multidict<7.0,>=4.5
  Downloading multidict-6.0.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (114 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 114.5/114.5 KB 2.5 MB/s eta 0:00:00
Requirement already satisfied: async-timeout<5.0,>=4.0 in /usr/local/lib/python3.10/dist-packages (from aiohttp>=3.7.4->black) (4.0.2)
Collecting yarl<2.0,>=1.0
  Downloading yarl-1.9.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (301 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 301.6/301.6 KB 1.7 MB/s eta 0:00:00
Collecting aiosignal>=1.1.2
  Downloading aiosignal-1.3.1-py3-none-any.whl (7.6 kB)
Collecting attrs>=17.3.0
  Using cached attrs-23.1.0-py3-none-any.whl (61 kB)
Collecting frozenlist>=1.1.1
  Downloading frozenlist-1.4.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (225 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 225.7/225.7 KB 2.1 MB/s eta 0:00:00
Requirement already satisfied: idna>=2.0 in /usr/lib/python3/dist-packages (from yarl<2.0,>=1.0->aiohttp>=3.7.4->black) (3.3)
Installing collected packages: typing-extensions, pathspec, mypy-extensions, multidict, frozenlist, attrs, yarl, aiosignal, aiohttp, black
Successfully installed aiohttp-3.9.1 aiosignal-1.3.1 attrs-23.1.0 black-23.12.0 frozenlist-1.4.0 multidict-6.0.4 mypy-extensions-1.0.0 pathspec-0.12.1 typing-extensions-4.9.0 yarl-1.9.4
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ black --version
black, 23.12.0 (compiled: yes)
Python (CPython) 3.10.12
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git commit -m "rmv website redirect"
reformatted /home/frappe/frappe-bench/apps/drive/drive/drive/doctype/drive_entity_log/test_drive_entity_log.py
reformatted /home/frappe/frappe-bench/apps/drive/drive/hooks.py

All done! ✨ 🍰 ✨
2 files reformatted, 47 files left unchanged.

> frontend@0.0.0 precommit
> pretty-quick --staged

🔍  Finding changed files since git revision 56b9745.
🎯  Found 0 changed files.
✅  Everything is awesome!
[mydev 80be7af] rmv website redirect
 1 file changed, 1 insertion(+), 5 deletions(-)
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git push origin mydev
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git remote -v
upstream	https://github.com/Baljit998/F-Drive.git (fetch)
upstream	https://github.com/Baljit998/F-Drive.git (push)
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git add origin git@github.com:Baljit998/F-Drive.git
fatal: pathspec 'origin' did not match any files
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git remote add git@github.com:Baljit998/F-Drive.git
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git remote add origin git@github.com:Baljit998/F-Drive.git
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ git push origin mydev
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 352 bytes | 352.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To github.com:Baljit998/F-Drive.git
   56b9745..80be7af  mydev -> mydev
frappe@baljit-ThinkPad-T460:~/frappe-bench/apps/drive$ 

