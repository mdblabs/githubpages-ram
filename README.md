This repository has been forked from:
[this one.](https://github.com/kappataumu/vagrant-up-github-pages)

It has been modified to include REPO variable on the Vagrantfile itself (instead of an environment variable).

How-To
=====
1. Clone the repo:
```
git clone https://github.com/mdblabs/githubpages-ram.git
```
2. Enter githubpages-ram directory, and edit the Vagrantfile, in order to add the REPO tag:
```
cd githubpages-ram
vim Vagrantfile
```
In Windows, you can use your favorite text editor.

3. Add the github pages REPO address, in line 6:
```
REPO = "https://github.com/user/myexamplepage.github.io"
```
Save it, and close it.

4. Run Vagrant and provision:
```
vagrant up
```

A www folder will be created on your relative folder.it's  path can also be edited on the Vagrantfile (line 7, FOLDER tag).

Once Vagrant is finished, you can visit your local webpage copy (by default on port 4000):

```
http://localhost:4000
``` 

You can now edit your page as usual. Once any file is modified, inside thw www folder, the local copy will be updated. Then, you can update the remote repository, by using git as usual.
