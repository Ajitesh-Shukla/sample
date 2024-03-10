Steps to use github lfs for adding large files (limit 2 GB):

1) Follow this to install git lfs https://docs.github.com/en/repositories/working-with-files/managing-large-files/installing-git-large-file-storage (For mac it's just brew install git-lfs)
2) Move to your existing directory locally, open terminal there, do these:
3) git init
4) git lfs install                           (Cmnt: This initializes git lfs for current work, does not install, just like git init)
5) git remote add origin (Your repo link)    
6) git branch -M main                        (Cmnt: Or your branch)
7) git lfs track "*.mdf"                     (Cmnt: Can add more extensions as well, add those you wanna track)
8) git add .gitattributes                    (Cmnt: After last step, a .gitattributes hidden file was created, stage that for commit, it includes info about all your large files)
9) git add (file path locally)
10) git add .                                 (Cmnt: It is possible to skip last step and just do this, to add all files at once)
11) git commit -m "large file commit"
12) git push origin main




