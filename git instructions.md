
#make sure to register with github and substitue below appropriately.

a@star ~
$ ssh-keygen -t rsa -b 4096 -C "jstar.github@gmail.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/home/a/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /home/a/.ssh/id_rsa.
Your public key has been saved in /home/a/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:l0PVA3buPlv4RIoA3UhQO509cQQKoEpq2tNx188gKdE jstar.github@gmail.com
The key's randomart image is:
+---[RSA 4096]----+
|        o++ +o+oo|
|       o o O *oo |
|    . o E * = +. |
|   o . . = o . . |
|  o o o S B   . .|
| + . o o o * o + |
|. o .       + = o|
|   .           * |
|              . .|
+----[SHA256]-----+

a@star ~
$ ssh-add ~/.ssh/id_rsa
Identity added: /home/a/.ssh/id_rsa (/home/a/.ssh/id_rsa)

a@star ~
$ clip < ~/.ssh/id_rsa.pub

a@star ~
$ echo "# cryptozombies" >> README.md

a@star ~
$ git init
Reinitialized existing Git repository in /home/a/.git/

a@star ~
$ git config user.name "jstargithub"

a@star ~
$ git config user.email "jstar.github@gmail.com"

a@star ~
$ git remote add origin git@github.com:jstargithub/cryptozombies.git

a@star ~
$ git clone https://github.com/jstargithub/cryptozombies
Cloning into 'cryptozombies'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
Checking connectivity... done.

a@star ~
$ cd cryptozombies/

$ echo "# cryptozombies" >> README.md

a@star ~
$ git add *

a@star ~
$ git commit -m "this is it"
[master (root-commit) 6e33573] this is it
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

a@star ~/cryptozombies
$ git push origin master
Username for 'https://github.com':
Password for 'https://jstar.github@gmail.com@github.com':
Counting objects: 1, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (1/1), done.
Writing objects: 100% (1/1), 280 bytes | 0 bytes/s, done.
Total 1 (delta 0), reused 0 (delta 0)
To https://github.com/jstargithub/cryptozombies
   6e33573..89b030c  master -> master
