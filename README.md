<<<<<<< HEAD
# lab02
export GITHUB_USERNAME=samchik7          
export GITHUB_EMAIL=s4gabalyan@yandex.ru   
export GITHUB_TOKEN=token
alias edit=nano
cd ${GITHUB_USERNAME}/workspace
source scripts/activate




mkdir ~/.config
mkdir: /Users/sam/.config: File exists
cat > ~/.config/hub <<EOF
github.com:
- user: ${GITHUB_USERNAME}
  oauth_token: ${GITHUB_TOKEN}
  protocol: https
EOF
git config --global hub.protocol https




mkdir projects/lab02 && cd projects/lab02
git init
Initialized empty Git repository in /Users/sam/samchik7/workspace/projects/lab02/.git/
git config --global user.name ${GITHUB_USERNAME}
git config -e --global
git remote add origin https://github.com/${GITHUB_USERNAME}/lab02.git
error: remote origin already exists.
touch README.md
git status
On branch main
nothing to commit, working tree clean
git add README.md
git commit -m"added README.md"
On branch main
nothing to commit, working tree clean
git push origin main  
Username for 'https://github.com': samchik7
Password for 'https://samchik7@github.com': 
Everything up-to-date





git pull origin main  
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 976 bytes | 325.00 KiB/s, done.
From https://github.com/samchik7/lab02
 * branch            main       -> FETCH_HEAD
   d6e6cc2..c5fdd96  main       -> origin/main
Updating d6e6cc2..c5fdd96
Fast-forward
 .gitignore | 4 ++++
 1 file changed, 4 insertions(+)
 create mode 100644 .gitignore
git log
commit c5fdd96194752ffa67822698ef5dc9f6fd23f7c1 (HEAD -> main, origin/main)
Author: samchik7 <s4gabalyan@yandex.ru>
Date:   Mon Mar 10 18:38:47 2025 +0300

    .gitignore

commit d6e6cc2886bd779627ce5ba279652a6ab61c25d4
Author: samchik7 <s4gabalyan@yandex.ru>
Date:   Mon Mar 10 13:55:04 2025 +0300

    Initial commit





mkdir sources
mkdir include
mkdir examples
cat > sources/print.cpp <<EOF
#include <print.hpp>

void print(const std::string& text, std::ostream& out)
{
  out << text;
}

void print(const std::string& text, std::ofstream& out)
{
  out << text;
}
EOF




cat > include/print.hpp <<EOF
#include <fstream>
#include <iostream>
#include <string>

void print(const std::string& text, std::ofstream& out);
void print(const std::string& text, std::ostream& out = std::cout);
EOF




cat > examples/example1.cpp <<EOF
#include <print.hpp>

int main(int argc, char** argv)
{
  print("hello");
}
EOF




cat > examples/example2.cpp <<EOF
#include <print.hpp>

#include <fstream>

int main(int argc, char** argv)
{
  std::ofstream file("log.txt");
  print(std::string("hello"), file);
}
EOF



git add .
git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   examples/example1.cpp
	new file:   examples/example2.cpp
	new file:   include/print.hpp
	new file:   sources/print.cpp
it commit -m"added sources"
[main 693db45] added sources
 4 files changed, 32 insertions(+)
 create mode 100644 examples/example1.cpp
 create mode 100644 examples/example2.cpp
 create mode 100644 include/print.hpp
 create mode 100644 sources/print.cpp
git push origin main  
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (9/9), 960 bytes | 960.00 KiB/s, done.
Total 9 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/samchik7/lab02.git
   c5fdd96..693db45  main -> main
   




=======
# lab03
>>>>>>> 2a32019fa8b14a21dfd0f4f019dc63a33bed16da
