C:\Users\91987>mkdir expr8

C:\Users\91987>cd expr8

C:\Users\91987\expr8>git init
Initialized empty Git repository in C:/Users/91987/expr8/.git/

C:\Users\91987\expr8>8a.txt

C:\Users\91987\expr8>8b.txt

C:\Users\91987\expr8>git checkout -b fb1
Switched to a new branch 'fb1'

C:\Users\91987\expr8>8a.txt

C:\Users\91987\expr8>git add .

C:\Users\91987\expr8>git commit -m "first commit "
[fb1 (root-commit) 5045090] first commit
 2 files changed, 3 insertions(+)
 create mode 100644 8a.txt
 create mode 100644 8b.txt

C:\Users\91987\expr8>8b.txt

C:\Users\91987\expr8>git add .

C:\Users\91987\expr8>git commit -m "second commit "
[fb1 793a10d] second commit
 1 file changed, 1 insertion(+)

C:\Users\91987\expr8>8a.txt

C:\Users\91987\expr8>git add .

C:\Users\91987\expr8>git commit -m "third"
On branch fb1
nothing to commit, working tree clean

C:\Users\91987\expr8>8a.txt

C:\Users\91987\expr8>git commit -m "third"
On branch fb1
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   8a.txt

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\91987\expr8>git add .

C:\Users\91987\expr8>git commit -m "third"
[fb1 f4acb09] third
 1 file changed, 1 insertion(+)

C:\Users\91987\expr8>8b.txt

C:\Users\91987\expr8>git add .

C:\Users\91987\expr8>git commit -m "fourth"
[fb1 5c6f27a] fourth
 1 file changed, 1 insertion(+)

C:\Users\91987\expr8>git log
commit 5c6f27a66f04b5712408d76cd46f250106930a4a (HEAD -> fb1)
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:13:06 2024 +0530

    fourth

commit f4acb09966fc2fb125108b4aa2c2ca75455c7205
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:12:22 2024 +0530

    third

commit 793a10deee2e24033f4ab4ff98413b8552670e71
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:10:52 2024 +0530

    second commit

commit 5045090d932630fb36d2ce7417e57455ea3eea30
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:10:07 2024 +0530

    first commit

C:\Users\91987\expr8>git tag 2.0  f4acb09966fc2fb125108b4aa2c2ca75455c7205

C:\Users\91987\expr8>git log
commit 5c6f27a66f04b5712408d76cd46f250106930a4a (HEAD -> fb1)
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:13:06 2024 +0530

    fourth

commit f4acb09966fc2fb125108b4aa2c2ca75455c7205 (tag: 2.0)
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:12:22 2024 +0530

    third

commit 793a10deee2e24033f4ab4ff98413b8552670e71
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:10:52 2024 +0530

    second commit

commit 5045090d932630fb36d2ce7417e57455ea3eea30
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:10:07 2024 +0530

    first commit

C:\Users\91987\expr8>git tag -d f4acb09966fc2fb125108b4aa2c2ca75455c7205
error: tag 'f4acb09966fc2fb125108b4aa2c2ca75455c7205' not found.

C:\Users\91987\expr8>git tag -d 2.0
Deleted tag '2.0' (was f4acb09)

C:\Users\91987\expr8>git log
commit 5c6f27a66f04b5712408d76cd46f250106930a4a (HEAD -> fb1)
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:13:06 2024 +0530

    fourth

commit f4acb09966fc2fb125108b4aa2c2ca75455c7205
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:12:22 2024 +0530

    third

commit 793a10deee2e24033f4ab4ff98413b8552670e71
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:10:52 2024 +0530

    second commit

commit 5045090d932630fb36d2ce7417e57455ea3eea30
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:10:07 2024 +0530

    first commit

C:\Users\91987\expr8>git tag 3.0

C:\Users\91987\expr8>git log
commit 5c6f27a66f04b5712408d76cd46f250106930a4a (HEAD -> fb1, tag: 3.0)
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:13:06 2024 +0530

    fourth

commit f4acb09966fc2fb125108b4aa2c2ca75455c7205
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:12:22 2024 +0530

    third

commit 793a10deee2e24033f4ab4ff98413b8552670e71
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:10:52 2024 +0530

    second commit

commit 5045090d932630fb36d2ce7417e57455ea3eea30
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:10:07 2024 +0530

    first commit

C:\Users\91987\expr8>git tag -d

C:\Users\91987\expr8>git log
commit 5c6f27a66f04b5712408d76cd46f250106930a4a (HEAD -> fb1, tag: 3.0)
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:13:06 2024 +0530

    fourth

commit f4acb09966fc2fb125108b4aa2c2ca75455c7205
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:12:22 2024 +0530

    third

commit 793a10deee2e24033f4ab4ff98413b8552670e71
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:10:52 2024 +0530

    second commit

commit 5045090d932630fb36d2ce7417e57455ea3eea30
Author: mayuresh041 <mayuresh0pathak4@gmail.com>
Date:   Sun Mar 3 22:10:07 2024 +0530

    first commit

C:\Users\91987\expr8>
