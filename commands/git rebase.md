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

