# test-git
test-git


============================||
                            ||
                            ||
                            ||
   Hello Git                ||
                            ||
                            ||
                            ||
============================||


kk@kk:~$ sudo su -
[sudo] password for kk: 
┌─[root@kk]─[~]
└──╼ #lss
Command 'lss' not found, but there are 16 similar ones.
┌─[✗]─[root@kk]─[~]
└──╼ #ls
git-devops  snap
┌─[root@kk]─[~]
└──╼ #rm -rf git-devops/
┌─[root@kk]─[~]
└──╼ #ll
total 80
drwx------  8 root root  4096 Dec 15 19:37 ./
drwxr-xr-x 23 root root  4096 Dec 15 16:49 ../
drwxr-xr-x  3 root root  4096 Dec 11 20:16 .anydesk/
-rw-------  1 root root  8367 Dec 15 16:51 .bash_history
-rw-r--r--  1 root root  4713 Dec 11 20:40 .bashrc
-rw-r--r--  1 root root  3106 Apr 22  2024 .bashrc-org
drwx------  2 root root  4096 Aug 27 21:09 .cache/
drwx------  4 root root  4096 Dec 15 16:49 .config/
drwxr-xr-x  7 root root  4096 Dec 15 12:51 .git/
-rw-r--r--  1 root root   123 Dec 15 12:13 .gitconfig
-rw-------  1 root root    20 Dec 15 12:53 .lesshst
-rw-r--r--  1 root root   161 Apr 22  2024 .profile
drwx------  7 root root  4096 Dec 11 14:24 snap/
drwx------  2 root root  4096 Dec 10 20:20 .ssh/
-rw-------  1 root root 12189 Dec 15 16:38 .viminfo
┌─[root@kk]─[~]
└──╼ #mkdir git
┌─[root@kk]─[~]
└──╼ #cd git/
┌─[root@kk]─[~/git]
└──╼ #ls
┌─[root@kk]─[~/git]
└──╼ #git -v
git version 2.43.0
┌─[root@kk]─[~/git]
└──╼ #git clone https://github.com/devcomeops/test-git.git
Cloning into 'test-git'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.
┌─[root@kk]─[~/git]
└──╼ #als
Command 'als' not found, but can be installed with:
apt install atool
┌─[✗]─[root@kk]─[~/git]
└──╼ #ls
test-git
┌─[root@kk]─[~/git]
└──╼ #ll
total 12
drwxr-xr-x 3 root root 4096 Dec 15 19:38 ./
drwx------ 9 root root 4096 Dec 15 19:37 ../
drwxr-xr-x 3 root root 4096 Dec 15 19:38 test-git/
┌─[root@kk]─[~/git]
└──╼ #git init
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
Initialized empty Git repository in /root/git/.git/
┌─[root@kk]─[~/git]
└──╼ #ll
total 16
drwxr-xr-x 4 root root 4096 Dec 15 19:38 ./
drwx------ 9 root root 4096 Dec 15 19:37 ../
drwxr-xr-x 7 root root 4096 Dec 15 19:38 .git/
drwxr-xr-x 3 root root 4096 Dec 15 19:38 test-git/
┌─[root@kk]─[~/git]
└──╼ #cat .git/config 
[core]
	repositoryformatversion = 0
	filemode = true
	bare = false
	logallrefupdates = true
┌─[root@kk]─[~/git]
└──╼ #git remote add origin https://github.com/devcomeops/test-git.git
┌─[root@kk]─[~/git]
└──╼ #git remote -v
origin	https://github.com/devcomeops/test-git.git (fetch)
origin	https://github.com/devcomeops/test-git.git (push)
┌─[root@kk]─[~/git]
└──╼ #git branch
┌─[root@kk]─[~/git]
└──╼ #git add .
warning: adding embedded git repository: test-git
hint: You've added another git repository inside your current repository.
hint: Clones of the outer repository will not contain the contents of
hint: the embedded repository and will not know how to obtain it.
hint: If you meant to add a submodule, use:
hint: 
hint: 	git submodule add <url> test-git
hint: 
hint: If you added this path by mistake, you can remove it from the
hint: index with:
hint: 
hint: 	git rm --cached test-git
hint: 
hint: See "git help submodule" for more information.
┌─[root@kk]─[~/git]
└──╼ #git commit -m "modute"
[master (root-commit) 3c64e64] modute
 1 file changed, 1 insertion(+)
 create mode 160000 test-git
┌─[root@kk]─[~/git]
└──╼ #git push origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/devcomeops/test-git.git'
┌─[✗]─[root@kk]─[~/git]
└──╼ #cd
┌─[root@kk]─[~]
└──╼ #
┌─[root@kk]─[~]
└──╼ #
┌─[root@kk]─[~]
└──╼ #cd /home/kk/
.anydesk/  Desktop/   .gnupg/    Pictures/  snap/      Videos/    
.cache/    Documents/ .local/    .pki/      .ssh/      
.config/   Downloads/ Music/     Public/    Templates/ 
┌─[root@kk]─[~]
└──╼ #mount
mount             mount.fuse3       mount.ntfs        mountpoint
mount.fuse        mount.lowntfs-3g  mount.ntfs-3g     mountsnoop-bpfcc
┌─[root@kk]─[~]
└──╼ #mount
mount             mount.fuse3       mount.ntfs        mountpoint
mount.fuse        mount.lowntfs-3g  mount.ntfs-3g     mountsnoop-bpfcc
┌─[root@kk]─[~]
└──╼ #mount -a /dev/sda
┌─[root@kk]─[~]
└──╼ #df -h
Filesystem      Size  Used Avail Use% Mounted on
tmpfs           2.4G  2.3M  2.4G   1% /run
/dev/nvme0n1p2  916G  148G  722G  17% /
tmpfs            12G   18M   12G   1% /dev/shm
tmpfs           5.0M   12K  5.0M   1% /run/lock
tmpfs           2.4G  236K  2.4G   1% /run/user/1000
┌─[root@kk]─[~]
└──╼ #lsblk 
NAME        MAJ:MIN RM   SIZE RO TYPE MOUNTPOINTS
loop0         7:0    0     4K  1 loop /snap/bare/5
loop1         7:1    0   124M  1 loop /snap/cherrytree/81
loop2         7:2    0  74.3M  1 loop /snap/core22/1564
loop3         7:3    0  73.9M  1 loop /snap/core22/1722
loop4         7:4    0 273.7M  1 loop /snap/firefox/5437
loop5         7:5    0  66.2M  1 loop /snap/core24/609
loop6         7:6    0  10.7M  1 loop /snap/firmware-updater/127
loop7         7:7    0 269.8M  1 loop /snap/firefox/4793
loop8         7:8    0  11.1M  1 loop /snap/firmware-updater/147
loop9         7:9    0 505.1M  1 loop /snap/gnome-42-2204/176
loop10        7:10   0 406.3M  1 loop /snap/gnome-46-2404/48
loop11        7:11   0  91.7M  1 loop /snap/gtk-common-themes/1535
loop12        7:12   0 211.5M  1 loop /snap/mesa-2404/143
loop13        7:13   0  10.5M  1 loop /snap/snap-store/1173
loop14        7:14   0  10.8M  1 loop /snap/snap-store/1244
loop15        7:15   0  38.8M  1 loop /snap/snapd/21759
loop16        7:16   0  44.3M  1 loop /snap/snapd/23258
loop17        7:17   0   568K  1 loop /snap/snapd-desktop-integration/253
loop18        7:18   0   500K  1 loop /snap/snapd-desktop-integration/178
sda           8:0    0   1.8T  0 disk 
└─sda1        8:1    0   1.8T  0 part 
nvme0n1     259:0    0 931.5G  0 disk 
├─nvme0n1p1 259:1    0     1M  0 part 
└─nvme0n1p2 259:2    0 931.5G  0 part /
┌─[root@kk]─[~]
└──╼ #cat /etc/fstab 
# /etc/fstab: static file system information.
#
# Use 'blkid' to print the universally unique identifier for a
# device; this may be used with UUID= as a more robust way to name devices
# that works even if disks are added and removed. See fstab(5).
#
# <file system> <mount point>   <type>  <options>       <dump>  <pass>
# / was on /dev/nvme0n1p2 during curtin installation
/dev/disk/by-uuid/ae918f71-81ad-4c80-95c6-a60087064192 / ext4 defaults 0 1
/swap.img	none	swap	sw	0	0
┌─[root@kk]─[~]
└──╼ #cd /media/kk/
┌─[root@kk]─[/media/kk]
└──╼ #ls
┌─[root@kk]─[/media/kk]
└──╼ #cd /mnt/
┌─[root@kk]─[/mnt]
└──╼ #ll
total 8
drwxr-xr-x  2 root root 4096 Aug 27 21:07 ./
drwxr-xr-x 23 root root 4096 Dec 15 16:49 ../
┌─[root@kk]─[/mnt]
└──╼ #lsblk 
NAME        MAJ:MIN RM   SIZE RO TYPE MOUNTPOINTS
loop0         7:0    0     4K  1 loop /snap/bare/5
loop1         7:1    0   124M  1 loop /snap/cherrytree/81
loop2         7:2    0  74.3M  1 loop /snap/core22/1564
loop3         7:3    0  73.9M  1 loop /snap/core22/1722
loop4         7:4    0 273.7M  1 loop /snap/firefox/5437
loop5         7:5    0  66.2M  1 loop /snap/core24/609
loop6         7:6    0  10.7M  1 loop /snap/firmware-updater/127
loop7         7:7    0 269.8M  1 loop /snap/firefox/4793
loop8         7:8    0  11.1M  1 loop /snap/firmware-updater/147
loop9         7:9    0 505.1M  1 loop /snap/gnome-42-2204/176
loop10        7:10   0 406.3M  1 loop /snap/gnome-46-2404/48
loop11        7:11   0  91.7M  1 loop /snap/gtk-common-themes/1535
loop12        7:12   0 211.5M  1 loop /snap/mesa-2404/143
loop13        7:13   0  10.5M  1 loop /snap/snap-store/1173
loop14        7:14   0  10.8M  1 loop /snap/snap-store/1244
loop15        7:15   0  38.8M  1 loop /snap/snapd/21759
loop16        7:16   0  44.3M  1 loop /snap/snapd/23258
loop17        7:17   0   568K  1 loop /snap/snapd-desktop-integration/253
loop18        7:18   0   500K  1 loop /snap/snapd-desktop-integration/178
sda           8:0    0   1.8T  0 disk 
└─sda1        8:1    0   1.8T  0 part /mnt/2b8bd7ee-4132-4ba2-90d6-2e07783e7108
nvme0n1     259:0    0 931.5G  0 disk 
├─nvme0n1p1 259:1    0     1M  0 part 
└─nvme0n1p2 259:2    0 931.5G  0 part /
┌─[root@kk]─[/mnt]
└──╼ #cd /mnt/2b8bd7ee-4132-4ba2-90d6-2e07783e7108/
┌─[root@kk]─[/mnt/2b8bd7ee-4132-4ba2-90d6-2e07783e7108]
└──╼ #ls
Downloads  kk-Backup  lost+found  SEGATE  WINDOWS.pem
┌─[root@kk]─[/mnt/2b8bd7ee-4132-4ba2-90d6-2e07783e7108]
└──╼ #cd
┌─[root@kk]─[~]
└──╼ #
┌─[root@kk]─[~]
└──╼ #
┌─[root@kk]─[~]
└──╼ #
┌─[root@kk]─[~]
└──╼ #cd git/
┌─[root@kk]─[~/git]
└──╼ #ls
test-git
┌─[root@kk]─[~/git]
└──╼ #ll
total 16
drwxr-xr-x 4 root root 4096 Dec 15 19:38 ./
drwx------ 9 root root 4096 Dec 15 19:39 ../
drwxr-xr-x 8 root root 4096 Dec 15 19:40 .git/
drwxr-xr-x 3 root root 4096 Dec 15 19:38 test-git/
┌─[root@kk]─[~/git]
└──╼ #git remote add origin https://github.com/devcomeops/test-git.git
error: remote origin already exists.
┌─[✗]─[root@kk]─[~/git]
└──╼ #git remote -v
origin	https://github.com/devcomeops/test-git.git (fetch)
origin	https://github.com/devcomeops/test-git.git (push)
┌─[root@kk]─[~/git]
└──╼ #git pull origin main
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 853 bytes | 284.00 KiB/s, done.
From https://github.com/devcomeops/test-git
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint: 
hint:   git config pull.rebase false  # merge
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
┌─[✗]─[root@kk]─[~/git]
└──╼ #cd test-git/
┌─[root@kk]─[~/git/test-git]
└──╼ #ls
README.md
┌─[root@kk]─[~/git/test-git]
└──╼ #ll
total 16
drwxr-xr-x 3 root root 4096 Dec 15 19:38 ./
drwxr-xr-x 4 root root 4096 Dec 15 19:38 ../
drwxr-xr-x 8 root root 4096 Dec 15 19:38 .git/
-rw-r--r-- 1 root root   20 Dec 15 19:38 README.md
┌─[root@kk]─[~/git/test-git]
└──╼ #git remote -v
origin	https://github.com/devcomeops/test-git.git (fetch)
origin	https://github.com/devcomeops/test-git.git (push)
┌─[root@kk]─[~/git/test-git]
└──╼ #echo "Hello git" > test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #ll
total 20
drwxr-xr-x 3 root root 4096 Dec 15 19:46 ./
drwxr-xr-x 4 root root 4096 Dec 15 19:38 ../
drwxr-xr-x 8 root root 4096 Dec 15 19:38 .git/
-rw-r--r-- 1 root root   20 Dec 15 19:38 README.md
-rw-r--r-- 1 root root   10 Dec 15 19:46 test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #git add .
┌─[root@kk]─[~/git/test-git]
└──╼ #git commit -m "test"
[main 86cf328] test
 1 file changed, 1 insertion(+)
 create mode 100644 test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #git push origin main
Username for 'https://github.com': devcomeops
Password for 'https://devcomeops@github.com': 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 276 bytes | 276.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/devcomeops/test-git.git
   449ab8b..86cf328  main -> main
┌─[root@kk]─[~/git/test-git]
└──╼ #ls
README.md  test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #mkdir test-push
┌─[root@kk]─[~/git/test-git]
└──╼ #git add .
┌─[root@kk]─[~/git/test-git]
└──╼ #git commit -m "push"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
┌─[✗]─[root@kk]─[~/git/test-git]
└──╼ #git push origin main
Username for 'https://github.com': devcomeops
Password for 'https://devcomeops@github.com': 
Everything up-to-date
┌─[root@kk]─[~/git/test-git]
└──╼ #git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
┌─[root@kk]─[~/git/test-git]
└──╼ #git log
commit 86cf32849842f6673793dcf023713dced4f523b7 (HEAD -> main, origin/main, origin/HEAD)
Author: devcomeops <devcomeops@gmail.com>
Date:   Sun Dec 15 19:47:00 2024 +0530

    test

commit 449ab8b872690da2f717965df444f486cdf59e2b
Author: devcomeops <devcomeops@gmail.com>
Date:   Sun Dec 15 16:33:52 2024 +0530

    Initial commit
┌─[root@kk]─[~/git/test-git]
└──╼ #ls
README.md  test-push  test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #ll
total 24
drwxr-xr-x 4 root root 4096 Dec 15 19:48 ./
drwxr-xr-x 4 root root 4096 Dec 15 19:38 ../
drwxr-xr-x 8 root root 4096 Dec 15 19:49 .git/
-rw-r--r-- 1 root root   20 Dec 15 19:38 README.md
drwxr-xr-x 2 root root 4096 Dec 15 19:48 test-push/
-rw-r--r-- 1 root root   10 Dec 15 19:46 test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #cd test-push/
┌─[root@kk]─[~/git/test-git/test-push]
└──╼ #ll
total 8
drwxr-xr-x 2 root root 4096 Dec 15 19:48 ./
drwxr-xr-x 4 root root 4096 Dec 15 19:48 ../
┌─[root@kk]─[~/git/test-git/test-push]
└──╼ #git init
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
Initialized empty Git repository in /root/git/test-git/test-push/.git/
┌─[root@kk]─[~/git/test-git/test-push]
└──╼ #git remote -v
┌─[root@kk]─[~/git/test-git/test-push]
└──╼ #git remote -v
┌─[root@kk]─[~/git/test-git/test-push]
└──╼ #ll
total 12
drwxr-xr-x 3 root root 4096 Dec 15 19:49 ./
drwxr-xr-x 4 root root 4096 Dec 15 19:48 ../
drwxr-xr-x 7 root root 4096 Dec 15 19:49 .git/
┌─[root@kk]─[~/git/test-git/test-push]
└──╼ #cat .git/config 
[core]
	repositoryformatversion = 0
	filemode = true
	bare = false
	logallrefupdates = true
┌─[root@kk]─[~/git/test-git/test-push]
└──╼ #ll
total 12
drwxr-xr-x 3 root root 4096 Dec 15 19:49 ./
drwxr-xr-x 4 root root 4096 Dec 15 19:48 ../
drwxr-xr-x 7 root root 4096 Dec 15 19:49 .git/
┌─[root@kk]─[~/git/test-git/test-push]
└──╼ #
┌─[root@kk]─[~/git/test-git/test-push]
└──╼ #ls
┌─[root@kk]─[~/git/test-git/test-push]
└──╼ #cd ..
┌─[root@kk]─[~/git/test-git]
└──╼ #ll
total 24
drwxr-xr-x 4 root root 4096 Dec 15 19:48 ./
drwxr-xr-x 4 root root 4096 Dec 15 19:38 ../
drwxr-xr-x 8 root root 4096 Dec 15 19:49 .git/
-rw-r--r-- 1 root root   20 Dec 15 19:38 README.md
drwxr-xr-x 3 root root 4096 Dec 15 19:49 test-push/
-rw-r--r-- 1 root root   10 Dec 15 19:46 test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #rm -rf test-push/
┌─[root@kk]─[~/git/test-git]
└──╼ #ll
total 20
drwxr-xr-x 3 root root 4096 Dec 15 20:00 ./
drwxr-xr-x 4 root root 4096 Dec 15 19:38 ../
drwxr-xr-x 8 root root 4096 Dec 15 19:49 .git/
-rw-r--r-- 1 root root   20 Dec 15 19:38 README.md
-rw-r--r-- 1 root root   10 Dec 15 19:46 test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #vim README.md 
┌─[root@kk]─[~/git/test-git]
└──╼ #ll
total 20
drwxr-xr-x 3 root root 4096 Dec 15 20:02 ./
drwxr-xr-x 4 root root 4096 Dec 15 19:38 ../
drwxr-xr-x 8 root root 4096 Dec 15 19:49 .git/
-rw-r--r-- 1 root root  301 Dec 15 20:02 README.md
-rw-r--r-- 1 root root   10 Dec 15 19:46 test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #git add .
┌─[root@kk]─[~/git/test-git]
└──╼ #git commit -m "local push"
[main 79ac2e9] local push
 1 file changed, 11 insertions(+)
┌─[root@kk]─[~/git/test-git]
└──╼ #gigt push origin main
Command 'gigt' not found, did you mean:
  command 'gist' from deb yorick (2.2.04+dfsg1-12)
  command 'git' from deb git (1:2.43.0-1ubuntu7.1)
  command 'gitg' from deb gitg (44-1)
Try: apt install <deb name>
┌─[✗]─[root@kk]─[~/git/test-git]
└──╼ #git push origin main
Username for 'https://github.com': devcomeops
Password for 'https://devcomeops@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 311 bytes | 155.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/devcomeops/test-git.git
   86cf328..79ac2e9  main -> main
┌─[root@kk]─[~/git/test-git]
└──╼ #pwd
/root/git/test-git
┌─[root@kk]─[~/git/test-git]
└──╼ #vim .gitignore
┌─[root@kk]─[~/git/test-git]
└──╼ #cat .gitignore 
.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #ll
total 24
drwxr-xr-x 3 root root 4096 Dec 15 20:05 ./
drwxr-xr-x 4 root root 4096 Dec 15 19:38 ../
drwxr-xr-x 8 root root 4096 Dec 15 20:02 .git/
-rw-r--r-- 1 root root    5 Dec 15 20:05 .gitignore
-rw-r--r-- 1 root root  301 Dec 15 20:02 README.md
-rw-r--r-- 1 root root   10 Dec 15 19:46 test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #touch demo.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #touch demo.mp3
┌─[root@kk]─[~/git/test-git]
└──╼ #touch demo.mp4
┌─[root@kk]─[~/git/test-git]
└──╼ #touch demo.java
┌─[root@kk]─[~/git/test-git]
└──╼ #
┌─[root@kk]─[~/git/test-git]
└──╼ #git add .
┌─[root@kk]─[~/git/test-git]
└──╼ #git commit -m "ignore .txt"
[main 70155b2] ignore .txt
 5 files changed, 1 insertion(+)
 create mode 100644 .gitignore
 create mode 100644 demo.java
 create mode 100644 demo.mp3
 create mode 100644 demo.mp4
 create mode 100644 demo.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #git push origin main
Username for 'https://github.com': devcomeops
Password for 'https://devcomeops@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 361 bytes | 120.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/devcomeops/test-git.git
   79ac2e9..70155b2  main -> main
┌─[root@kk]─[~/git/test-git]
└──╼ #vim .gitignore
┌─[root@kk]─[~/git/test-git]
└──╼ #
┌─[root@kk]─[~/git/test-git]
└──╼ #ls
demo.java  demo.mp3  demo.mp4  demo.txt  README.md  test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #rm -rf demo.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #ls
demo.java  demo.mp3  demo.mp4  README.md  test.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #touch demo.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #touch demoignore.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #touch demo1.vdi
┌─[root@kk]─[~/git/test-git]
└──╼ #git add .
┌─[root@kk]─[~/git/test-git]
└──╼ #git commit -m "demo.txt ignore"
[main d5cc171] demo.txt ignore
 2 files changed, 1 insertion(+), 1 deletion(-)
 create mode 100644 demo1.vdi
┌─[root@kk]─[~/git/test-git]
└──╼ #git status 
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
┌─[root@kk]─[~/git/test-git]
└──╼ #git log
commit d5cc171c931b494814a47438675b9abe385040fc (HEAD -> main)
Author: devcomeops <devcomeops@gmail.com>
Date:   Sun Dec 15 20:11:13 2024 +0530

    demo.txt ignore

commit 70155b24b5872174141ec7fc7aa5725444acdda3 (origin/main, origin/HEAD)
Author: devcomeops <devcomeops@gmail.com>
Date:   Sun Dec 15 20:06:33 2024 +0530

    ignore .txt

commit 79ac2e9057ee2c951ae466776c81d15015aac593
Author: devcomeops <devcomeops@gmail.com>
Date:   Sun Dec 15 20:02:33 2024 +0530

    local push

commit 86cf32849842f6673793dcf023713dced4f523b7
Author: devcomeops <devcomeops@gmail.com>
Date:   Sun Dec 15 19:47:00 2024 +0530

    test
┌─[root@kk]─[~/git/test-git]
└──╼ #git push origin main
Username for 'https://github.com': devcomeops
Password for 'https://devcomeops@github.com': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 292 bytes | 292.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/devcomeops/test-git.git
   70155b2..d5cc171  main -> main
┌─[root@kk]─[~/git/test-git]
└──╼ #cat .gitignore 
*.txt
┌─[root@kk]─[~/git/test-git]
└──╼ #

+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++




