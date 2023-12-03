- open aws and navigate to your account>security credential
- create a access key
- download the access key and secret
- configure it with our container or machine
````git
@abhiramdas99 ➜ /workspaces/devops-iac-terraform (main) $ aws configure
AWS Access Key ID [****************FF53]: AKIA6N5YMX3PMG*****
AWS Secret Access Key [****************b3ks]: xWd+Sx6P6PiKUHycEv5CpRZemdk8COMJ1n*****
Default region name [json]: ap-south-1
Default output format [None]: json
@abhiramdas99 ➜ /workspaces/devops-iac-terraform (main) $ 
````
- update container with  your git repo
```git
@abhiramdas99 ➜ /workspaces/devops-iac-terraform (main) $ git pull 
Already up to date.
@abhiramdas99 ➜ /workspaces/devops-iac-terraform (main) $ git add . 
@abhiramdas99 ➜ /workspaces/devops-iac-terraform (main) $ git status 
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .devcontainer/devcontainer.json

@abhiramdas99 ➜ /workspaces/devops-iac-terraform (main) $ git commit -m "commit .devcontainer"
[main cf1cb6b] commit .devcontainer
 1 file changed, 7 insertions(+)
 create mode 100644 .devcontainer/devcontainer.json
@abhiramdas99 ➜ /workspaces/devops-iac-terraform (main) $ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 505 bytes | 505.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/abhiramdas99/devops-iac-terraform
   195f723..cf1cb6b  main -> main
@abhiramdas99 ➜ /workspaces/devops-iac-terraform (main) $ 
```
