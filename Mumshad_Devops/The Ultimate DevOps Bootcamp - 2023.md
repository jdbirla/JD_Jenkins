# The Ultimate DevOps Bootcamp - 2023
- https://www.udemy.com/course/the-complete-devops-bootcamp/learn/lecture/28947472?start=15#overview
- LAB: https://kodekloud.com/courses/lab-course-the-complete-devops-bootcamp/
![image](https://user-images.githubusercontent.com/69948118/229992041-821a6888-bd3e-4353-9b27-4fa83d347927.png)
## Linux Basics
![image](https://user-images.githubusercontent.com/69948118/230009179-f8c641cc-5c46-409d-befb-40763ebdedab.png)
![image](https://user-images.githubusercontent.com/69948118/230009525-34ed67a4-e6b5-4d8b-8d73-2d739e2a0af8.png)
![image](https://user-images.githubusercontent.com/69948118/230009865-c900519d-5b17-4bd2-9e28-c5c8b745ae35.png)
![image](https://user-images.githubusercontent.com/69948118/230010439-505537d0-393a-4ae2-ab62-e8886d0f3b45.png)
```bash
thor@host01 ~$ pwd
/home/thor
thor@host01 ~$ ls /home/thor/test_dir/
dir1  dir2  dir3  test_file1.txt  test_file2.txt  test_file4.txt
thor@host01 ~$ cd ..
thor@host01 /home$ /home/thor/touch empty_file.txt
-bash: /home/thor/touch: No such file or directory
thor@host01 /home$ pwd
/home
thor@host01 /home$ cd thor/
thor@host01 ~$ ls
test_dir
thor@host01 ~$ touch empty_file.txt
thor@host01 ~$ cat contents_file.txt
cat: contents_file.txt: No such file or directory
thor@host01 ~$ cat > contents_file.txt 
This is not empty file
thor@host01 ~$ pwd
/home/thor
thor@host01 ~$ mkdir empty_dir
thor@host01 ~$ mkdir -p /home/thor/asia/india/bangalore
thor@host01 ~$ cp /home/thor/asia/bangalore.txt /home/thor/asia/india/bangalore/
thor@host01 ~$ pwd
/home/thor
thor@host01 ~$ cd /home/thor/asia/india/bangalore/
thor@host01 ~/asia/india/bangalore$ ls
bangalore.txt
thor@host01 ~/asia/india/bangalore$ cd ..
thor@host01 ~/asia/india$ cd /home/thor/
thor@host01 ~$ pwd
/home/thor
thor@host01 ~$ cp /home/thor/asia/india/bangalore /home/thor/
cp: omitting directory ‘/home/thor/asia/india/bangalore’
thor@host01 ~$ cp -r /home/thor/asia/india/bangalore /home/thor/
thor@host01 ~$ /home/thor/asia/
-bash: /home/thor/asia/: Is a directory
thor@host01 ~$ cd /home/thor/asia/
thor@host01 ~/asia$ ls
bangalore.txt  india
thor@host01 ~/asia$ rm bangalore.txt 
rm: remove write-protected regular file ‘bangalore.txt’? 
thor@host01 ~/asia$ rm bangalore.txt 
rm: remove write-protected regular file ‘bangalore.txt’? y
thor@host01 ~/asia$ rm /home/thor/asia/india/bangalore/
rm: cannot remove ‘/home/thor/asia/india/bangalore/’: Is a directory
thor@host01 ~/asia$ rm  -r /home/thor/asia/india/bangalore/
thor@host01 ~/asia$ ^C
```

### Vi Editor
![image](https://user-images.githubusercontent.com/69948118/230018090-4aa5ede9-3e82-48f1-8ac7-989bb5ca78fe.png)
![image](https://user-images.githubusercontent.com/69948118/230018312-5f7ae87a-44c8-4d24-b886-26363c1d20e0.png)
![image](https://user-images.githubusercontent.com/69948118/230018483-c317ecd9-b2e0-435d-9065-68fd7c118261.png)
![image](https://user-images.githubusercontent.com/69948118/230018652-6d9f35eb-794e-43c7-81a7-96ca86bce839.png)

### More Linux Command
![image](https://user-images.githubusercontent.com/69948118/230019227-dfc53eb0-3cc2-4f52-bf26-8352a4fd3381.png)
![image](https://user-images.githubusercontent.com/69948118/230019690-c625ab63-717f-4d43-8b56-b594a6ee8182.png)
![image](https://user-images.githubusercontent.com/69948118/230020058-6e524372-5c12-4a31-a462-72dee791ac94.png)
![image](https://user-images.githubusercontent.com/69948118/230020308-dcb3b9e7-366c-4340-89c3-cedda920cf85.png)

### Package Managers
![image](https://user-images.githubusercontent.com/69948118/230023988-e27b5863-6249-476b-bc72-088e28a567e4.png)
![image](https://user-images.githubusercontent.com/69948118/230024334-13261c9a-2d10-41d3-83cf-03484215cdaf.png)
![image](https://user-images.githubusercontent.com/69948118/230024601-fe5e8eda-4513-4405-97a3-bbb2982a3a63.png)
![image](https://user-images.githubusercontent.com/69948118/230025067-d193d009-e452-47e0-9c8b-014e908afcde.png)

### Services
![image](https://user-images.githubusercontent.com/69948118/230029520-8d1ee9f4-999d-445c-ae01-c9e06cea0e64.png)
![image](https://user-images.githubusercontent.com/69948118/230030132-5b2651c4-5e22-4fa8-b02c-9b4fa5b7e4ea.png)
![image](https://user-images.githubusercontent.com/69948118/230030573-fe29b50b-6a92-4491-bf0e-a5e49f2f9032.png)
![image](https://user-images.githubusercontent.com/69948118/230031020-5b6c4744-65d4-4363-bd86-a38e586d53f5.png)
![image](https://user-images.githubusercontent.com/69948118/230031250-170ee7b3-e8e3-42a2-8871-7ba6e975488c.png)
![image](https://user-images.githubusercontent.com/69948118/230031354-83b0f878-164a-42e4-9d96-b5da164fb27e.png)

## Networking 
![image](https://user-images.githubusercontent.com/69948118/230250347-2393af53-b6b6-4db5-8cef-f7d29c92a7e7.png)
![image](https://user-images.githubusercontent.com/69948118/230250630-6ebaf5e3-330c-4e8b-9990-1a6990b73667.png)
![image](https://user-images.githubusercontent.com/69948118/230250696-5bf5c1f4-d34f-41d1-88ad-53aff4aaab6c.png)
![image](https://user-images.githubusercontent.com/69948118/230250746-5a1a98de-5298-4aec-aec3-1dd8c4e56667.png)
![image](https://user-images.githubusercontent.com/69948118/230250808-23abc997-96d0-4e72-a643-fcf056aa0ea6.png)
![image](https://user-images.githubusercontent.com/69948118/230251291-1b1abb1b-dd86-4bab-b97f-908f77d86864.png)
![image](https://user-images.githubusercontent.com/69948118/230251420-16a61267-cbfe-4e28-a060-e360ee834073.png)
![image](https://user-images.githubusercontent.com/69948118/230251532-adcb67db-7a55-4d44-bdc8-042895ebab92.png)

### DNS
![image](https://user-images.githubusercontent.com/69948118/230256869-8dca3eee-fc0a-4fa0-9ae3-5577f97a7a81.png)
![image](https://user-images.githubusercontent.com/69948118/230257117-fe63d518-f59f-48db-a702-5ae9163dda37.png)
![image](https://user-images.githubusercontent.com/69948118/230257266-80394b51-c40e-449e-911e-5ff4a67a110d.png)
![image](https://user-images.githubusercontent.com/69948118/230257351-e0e542f9-cdda-4c18-b103-61fafdb19526.png)
![image](https://user-images.githubusercontent.com/69948118/230257810-9c793cf6-2936-43b5-a391-fa34301652d7.png)
![image](https://user-images.githubusercontent.com/69948118/230258006-3fdd124a-0223-49b4-996d-b9926c38f108.png)
![image](https://user-images.githubusercontent.com/69948118/230258192-3a89dff8-147b-4e17-9309-99fc8b0fe631.png)
![image](https://user-images.githubusercontent.com/69948118/230258457-b7489e41-725c-4bd0-9086-d49feb841799.png)
![image](https://user-images.githubusercontent.com/69948118/230258932-ec040b2c-192c-4177-a03b-b8cba3fd46d3.png)
![image](https://user-images.githubusercontent.com/69948118/230259154-a649de88-914d-4ee6-8e02-f7b581a61cee.png)
![image](https://user-images.githubusercontent.com/69948118/230259225-9f76021c-53ec-495f-beae-ba950120d956.png)

## Applications Basics
![image](https://user-images.githubusercontent.com/69948118/230262563-95ef9a15-09cc-414c-a749-e81d96409a2d.png)
```bash
thor@host01 ~$ java -version
openjdk version "1.8.0_242"
OpenJDK Runtime Environment (build 1.8.0_242-b08)
OpenJDK 64-Bit Server VM (build 25.242-b08, mixed mode)
thor@host01 ~$ ssh app01
The authenticity of host 'app01 (172.16.238.15)' can't be established.
ECDSA key fingerprint is SHA256:vxz89t3mPukTYcEHxvQEkOHoDcD42tkQ5UyP4F+cquk.
ECDSA key fingerprint is MD5:62:9c:a3:31:2b:a9:fd:85:69:1e:0a:28:1a:0f:62:6f.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added 'app01,172.16.238.15' (ECDSA) to the list of known hosts.
[thor@app01 ~]$ sudo curl https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz --output /opt/openjdk-13.0.2_linux-x64_bin.tar.gz
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  186M  100  186M    0     0  81.8M      0  0:00:02  0:00:02 --:--:-- 81.8M
[thor@app01 ~]$ ls
[thor@app01 ~]$ pwd
/home/thor
[thor@app01 ~]$ ls
[thor@app01 ~]$ /opt/
-bash: /opt/: Is a directory
[thor@app01 ~]$ ;s
-bash: syntax error near unexpected token `;'
[thor@app01 ~]$ cd /opt/
[thor@app01 opt]$ 
[thor@app01 opt]$ ls
openjdk-13.0.2_linux-x64_bin.tar.gz
[thor@app01 opt]$ sudo tar -xf openjdk-13.0.2_linux-x64_bin.tar.gz -C /opt/
[thor@app01 opt]$ java --version
-bash: java: command not found
[thor@app01 opt]$ jdk-13.0.2/bin/java --version
openjdk 13.0.2 2020-01-14
OpenJDK Runtime Environment (build 13.0.2+8)
OpenJDK 64-Bit Server VM (build 13.0.2+8, mixed mode, sharing)
[thor@app01 opt]$ 
[thor@app01 opt]$ export PATH=$PATH:/opt/jdk-13.0.2/bin/
[thor@app01 opt]$ echo PATH
PATH
[thor@app01 opt]$ echo $PATH
/usr/local/bin:/usr/bin:/usr/local/sbin:/usr/sbin:/home/thor/.local/bin:/home/thor/bin:/opt/jdk-13.0.2/bin/
[thor@app01 opt]$ 
```
### Build and Packages
![image](https://user-images.githubusercontent.com/69948118/230265180-18e33cde-3a50-4007-b55a-85da6bb20240.png)
![image](https://user-images.githubusercontent.com/69948118/230265549-a1455e53-621f-4a3e-9470-79856d1a4b7e.png)
![image](https://user-images.githubusercontent.com/69948118/230265579-4f0e54d3-9e81-4eb3-bcae-45c96ce2ea09.png)
```bash
thor@host01 /opt/app$ javac MyClass.java 
thor@host01 /opt/app$ ls
MyClass.class  MyClass.java
thor@host01 /opt/app$ cat MyClass.class 
9

java/lang/Object<init>()V



java/lang/SystemoutLjava/io/PrintStreamHello Kodekloud

java/io/PrintStreamprintln(Ljava/lang/String;)VMyClassCodeLineNumberTablemain([Ljava/lang/String;)V
SourceFile
          MyClass.java!*        %
thor@host01 /opt/app$ java MyClass
Hello Kodekloud
thor@host01 /opt/app$ javadoc -d MyClass.java 
javadoc: error - No modules, packages or classes specified.
1 error
thor@host01 /opt/app$ javadoc -d doc MyClass.java 
Loading source file MyClass.java...
Constructing Javadoc information...
Creating destination directory: "doc/"
Standard Doclet version 13.0.2
Building tree for all the packages and classes...
Generating doc/MyClass.html...
Generating doc/package-summary.html...
Generating doc/package-tree.html...
Generating doc/constant-values.html...
Building index for all the packages and classes...
Generating doc/overview-tree.html...
Generating doc/deprecated-list.html...
Generating doc/index-all.html...
Building index for all classes...
Generating doc/allclasses-index.html...
Generating doc/allpackages-index.html...
Generating doc/index.html...
Generating doc/help-doc.html...
thor@host01 /opt/app$ ls
doc  MyClass.class  MyClass.java
thor@host01 /opt/app$ cat doc/
cat: doc/: Is a directory
thor@host01 /opt/app$ cd doc/
thor@host01 /opt/app/doc$ ls
allclasses-index.html   element-list    member-search-index.js   package-search-index.js   resources   stylesheet.css
allpackages-index.html  help-doc.html   member-search-index.zip  package-search-index.zip  script-dir  type-search-index.js
constant-values.html    index-all.html  MyClass.html             package-summary.html      script.js   type-search-index.zip
deprecated-list.html    index.html      overview-tree.html       package-tree.html         search.js
thor@host01 /opt/app/doc$ curl index.html 
curl: (6) Could not resolve host: index.html; Unknown error
thor@host01 /opt/app/doc$ cat index.html 
```
- maven
```sh
thor@host01 /$ sudo yum install -y maven
thor@host01 /$ cd /opt/maven/my-app/
thor@host01 /opt/maven/my-app$ cd /opt/maven/my-app/; tree
.
├── pom.xml
└── src
    ├── main
    │   └── java
    │       └── com
    │           └── mycompany
    │               └── app
    │                   └── App.java
    └── test
        └── java
            └── com
                └── mycompany
                    └── app
                        └── AppTest.java
                        
thor@host01 /opt/maven/my-app$ sudo mvn package
thor@host01 /opt/maven/my-app$ ls
pom.xml  src  target
thor@host01 /opt/maven/my-app$ java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App
Hello World!
thor@host01 /opt/maven/my-app$ 
```
### NodeJS
![image](https://user-images.githubusercontent.com/69948118/230272450-8e7b9cfe-9f78-450f-9cca-021c309b4ec2.png)
![image](https://user-images.githubusercontent.com/69948118/230272525-de4db47c-8f59-4bbd-99e3-c5d516b2ef4c.png)
![image](https://user-images.githubusercontent.com/69948118/230273021-ed88e54e-28f7-468f-9041-c2943db38ece.png)
![image](https://user-images.githubusercontent.com/69948118/230273189-54bd2eb4-aec2-47e8-9fee-29f9f15d1ae6.png)
![image](https://user-images.githubusercontent.com/69948118/230273214-ff79c2e3-097e-4b7e-813f-56f42eba72c8.png)
![image](https://user-images.githubusercontent.com/69948118/230273380-f927fbe1-7599-49a4-b8ee-eb42e93b8aa4.png)
![image](https://user-images.githubusercontent.com/69948118/230273435-318e198a-23a4-43ef-bf4c-7c2bf92d2e49.png)

## Python 
![image](https://user-images.githubusercontent.com/69948118/230275150-bc73c4ae-8282-4070-9dc6-9e95fcc2a1ab.png)
![image](https://user-images.githubusercontent.com/69948118/230275393-63cb8fa5-3a06-4a37-ba8c-1f728a07c3ac.png)
![image](https://user-images.githubusercontent.com/69948118/230275717-80e96084-0b06-41d0-8482-c17a05e70b3f.png)
![image](https://user-images.githubusercontent.com/69948118/230276243-4741bfee-abcf-45ff-a122-2a64b4dc48c7.png)
![image](https://user-images.githubusercontent.com/69948118/230276380-909255a4-f4a7-47f6-9301-dfb503fe3105.png)
![image](https://user-images.githubusercontent.com/69948118/230276732-3e1f0312-3e18-4656-9247-05aca5d42c68.png)
![image](https://user-images.githubusercontent.com/69948118/230276867-25ced19c-de96-46b0-87e7-248a23a894d0.png)

## GIT Introduction
![image](https://user-images.githubusercontent.com/69948118/230292488-49770d1b-71bd-45c7-a3bd-9a5a3e5acee8.png)
![image](https://user-images.githubusercontent.com/69948118/230292724-b6d38f6b-42a5-41ea-aee1-5ab0a1fbfc61.png)
![image](https://user-images.githubusercontent.com/69948118/230292840-ed4ce4cf-b849-4ddc-8a77-93be398947b7.png)
![image](https://user-images.githubusercontent.com/69948118/230303565-d469b09e-994a-4410-8d8f-5ce4723ceaec.png)

## GIT Branches
![image](https://user-images.githubusercontent.com/69948118/230306650-88f427ee-7d7d-4124-b054-02672f421c24.png)
![image](https://user-images.githubusercontent.com/69948118/230306843-f78872ab-8143-483d-bd5b-00b651410403.png)
![image](https://user-images.githubusercontent.com/69948118/230307312-7ab964ef-4712-47d8-9977-1fcb0d6c3632.png)
![image](https://user-images.githubusercontent.com/69948118/230311536-07f7349e-eede-46ff-8609-f606dc49a112.png)
![image](https://user-images.githubusercontent.com/69948118/230311860-9ad87830-baa3-4d16-aaee-ca5b78722424.png)

## Remote Repo
![image](https://user-images.githubusercontent.com/69948118/230323005-6af45ed3-c864-463f-ba62-7f7097849168.png)
![image](https://user-images.githubusercontent.com/69948118/230323044-2fcc5732-ccd2-4d1b-a53b-b1ed1fcc9dc2.png)
![image](https://user-images.githubusercontent.com/69948118/230323181-d1502885-a0ca-4253-9375-a5331e77c1e3.png)
![image](https://user-images.githubusercontent.com/69948118/230323307-3e0aa93a-378e-4214-b0d8-dab1c07b7791.png)
![image](https://user-images.githubusercontent.com/69948118/230323512-3d7d0e2c-475c-4f5a-9ea2-2c96aa5e0db0.png)
![image](https://user-images.githubusercontent.com/69948118/230326656-a6027e0c-66cc-4dd5-bd5f-01a015d219f6.png)
![image](https://user-images.githubusercontent.com/69948118/230326743-a8003cba-3b8c-46b4-a2de-0c067f305386.png)
![image](https://user-images.githubusercontent.com/69948118/230326822-85c7dca6-5848-489d-adc9-ab8d19dc3ea9.png)
![image](https://user-images.githubusercontent.com/69948118/230327109-55f44f93-1aa6-45c0-b6a8-8a804be793e7.png)
![image](https://user-images.githubusercontent.com/69948118/230327264-f88eac0f-58e0-4930-8ea7-1b7057d1eb10.png)
![image](https://user-images.githubusercontent.com/69948118/230327399-b4973b4b-11d3-4d4c-a465-73ffc351ce2b.png)
![image](https://user-images.githubusercontent.com/69948118/230327422-1cf0f00c-4b33-40ad-a1ef-2019b86ae7e9.png)
![image](https://user-images.githubusercontent.com/69948118/230327539-8036e5dd-4ddc-4107-b709-d919d87119ca.png)
![image](https://user-images.githubusercontent.com/69948118/230327795-1c36c2ec-d777-4537-af69-b09948d80878.png)

## Jenkins Introduction
![image](https://user-images.githubusercontent.com/69948118/230336110-efdadd41-8d08-41af-8e1f-015a15c79f8d.png)
![image](https://user-images.githubusercontent.com/69948118/230336734-2c3026fb-4e47-464e-874f-6aba2f8a3ea8.png)
![image](https://user-images.githubusercontent.com/69948118/230336924-47014213-bc82-419f-b037-a26c3953a000.png)
![image](https://user-images.githubusercontent.com/69948118/230337457-e86596d5-2956-452c-8760-c39dae91bd2f.png)
![image](https://user-images.githubusercontent.com/69948118/230337759-dc368d9e-cea9-4484-bbfd-afc1417a8244.png)

```bash
jdwinlinux@DESKTOP-AS2FQOH:~$ sudo apt install openjdk-11-jdk
root@jdvmlinuxusr:~# curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
root@jdvmlinuxusr:~# echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
root@jdvmlinuxusr:~# sudo apt-get update
Ign:1 https://pkg.jenkins.io/debian-stable binary/ InRelease
Get:2 https://pkg.jenkins.io/debian-stable binary/ Release [2,044 B]
Get:3 https://pkg.jenkins.io/debian-stable binary/ Release.gpg [833 B]
Hit:4 http://in.archive.ubuntu.com/ubuntu jammy InRelease
Get:5 https://pkg.jenkins.io/debian-stable binary/ Packages [24.6 kB]
Hit:6 http://in.archive.ubuntu.com/ubuntu jammy-updates InRelease
Hit:7 http://in.archive.ubuntu.com/ubuntu jammy-backports InRelease
Hit:8 http://security.ubuntu.com/ubuntu jammy-security InRelease
Fetched 27.4 kB in 2s (12.5 kB/s)
Reading package lists... Done
root@jdvmlinuxusr:~# sudo apt-get install jenkins
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following NEW packages will be installed:
  jenkins
0 upgraded, 1 newly installed, 0 to remove and 3 not upgraded.
Need to get 97.7 MB of archives.
After this operation, 98.4 MB of additional disk space will be used.
Get:1 https://pkg.jenkins.io/debian-stable binary/ jenkins 2.387.2 [97.7 MB]
Fetched 97.7 MB in 30s (3,211 kB/s)
Selecting previously unselected package jenkins.
(Reading database ... 208726 files and directories currently installed.)
Preparing to unpack .../jenkins_2.387.2_all.deb ...
Unpacking jenkins (2.387.2) ...
Setting up jenkins (2.387.2) ...
Created symlink /etc/systemd/system/multi-user.target.wants/jenkins.service → /lib/systemd/system/jenkins.service.
root@jdvmlinuxusr:~# sudo apt-get install jenkins
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
jenkins is already the newest version (2.387.2).
0 upgraded, 0 newly installed, 0 to remove and 3 not upgraded.
root@jdvmlinuxusr:~# sudo systemctl start jenkins
root@jdvmlinuxusr:~# systemlctl status jenkins
Command 'systemlctl' not found, did you mean:
  command 'systemctl' from deb systemd (249.11-0ubuntu3.7)
  command 'systemctl' from deb systemctl (1.4.4181-1.1)
Try: apt install <deb name>
root@jdvmlinuxusr:~# systemctl status jenkins
● jenkins.service - Jenkins Continuous Integration Server
     Loaded: loaded (/lib/systemd/system/jenkins.service; enabled; vendor preset: enabled)
     Active: active (running) since Sat 2023-04-08 11:27:09 IST; 3min 47s ago
   Main PID: 7110 (java)
      Tasks: 42 (limit: 7210)
     Memory: 1.7G
        CPU: 1min 52.701s
     CGroup: /system.slice/jenkins.service
             └─7110 /usr/bin/java -Djava.awt.headless=true -jar /usr/share/java/jenkins.war --webroot=/var/cache/jenkins/war --httpPort=8080

Apr 08 11:26:13 jdvmlinuxusr jenkins[7110]: 5ac5938db28c40e4bac40ca2c08cbc38
Apr 08 11:26:13 jdvmlinuxusr jenkins[7110]: This may also be found at: /var/lib/jenkins/secrets/initialAdminPassword
Apr 08 11:26:13 jdvmlinuxusr jenkins[7110]: *************************************************************
Apr 08 11:26:13 jdvmlinuxusr jenkins[7110]: *************************************************************
Apr 08 11:26:13 jdvmlinuxusr jenkins[7110]: *************************************************************
Apr 08 11:27:08 jdvmlinuxusr jenkins[7110]: 2023-04-08 05:57:08.389+0000 [id=29]        INFO        jenkins.InitReactorRunner$1#onAttained: Completed initialization
Apr 08 11:27:09 jdvmlinuxusr jenkins[7110]: 2023-04-08 05:57:09.227+0000 [id=22]        INFO        hudson.lifecycle.Lifecycle#onReady: Jenkins is fully up and running
Apr 08 11:27:09 jdvmlinuxusr systemd[1]: Started Jenkins Continuous Integration Server.
Apr 08 11:27:10 jdvmlinuxusr jenkins[7110]: 2023-04-08 05:57:10.928+0000 [id=46]        INFO        h.m.DownloadService$Downloadable#load: Obtained the updated data file for hudson.tasks.Maven.MavenInstaller
Apr 08 11:27:10 jdvmlinuxusr jenkins[7110]: 2023-04-08 05:57:10.930+0000 [id=46]        INFO        hudson.util.Retrier#start: Performed the action check updates server successfully at the attempt #1
root@jdvmlinuxusr:~# sudo ufw allow 8080
Rules updated
Rules updated (v6)
root@jdvmlinuxusr:~# sudo ufw status
Status: inactive
root@jdvmlinuxusr:~#  exit
logout
jdvmlinuxusr@jdvmlinuxusr:~$ systemctl status jenkins
● jenkins.service - Jenkins Continuous Integration Server
     Loaded: loaded (/lib/systemd/system/jenkins.service; enabled; vendor preset: enabled)
     Active: active (running) since Sat 2023-04-08 11:27:09 IST; 8min ago
   Main PID: 7110 (java)
      Tasks: 42 (limit: 7210)
     Memory: 1.7G
        CPU: 1min 54.691s
     CGroup: /system.slice/jenkins.service
             └─7110 /usr/bin/java -Djava.awt.headless=true -jar /usr/share/java/jenkins.war --webroot=/var/cache/jenkins/war --httpPort=8080

Apr 08 11:26:13 jdvmlinuxusr jenkins[7110]: 5ac5938db28c40e4bac40ca2c08cbc38
Apr 08 11:26:13 jdvmlinuxusr jenkins[7110]: This may also be found at: /var/lib/jenkins/secrets/initialAdminPassword
Apr 08 11:26:13 jdvmlinuxusr jenkins[7110]: *************************************************************
Apr 08 11:26:13 jdvmlinuxusr jenkins[7110]: *************************************************************
Apr 08 11:26:13 jdvmlinuxusr jenkins[7110]: *************************************************************
Apr 08 11:27:08 jdvmlinuxusr jenkins[7110]: 2023-04-08 05:57:08.389+0000 [id=29]        INFO        jenkins.InitReactorRunner$1#onAttained: Completed initialization
Apr 08 11:27:09 jdvmlinuxusr jenkins[7110]: 2023-04-08 05:57:09.227+0000 [id=22]        INFO        hudson.lifecycle.Lifecycle#onReady: Jenkins is fully up and running
Apr 08 11:27:09 jdvmlinuxusr systemd[1]: Started Jenkins Continuous Integration Server.
Apr 08 11:27:10 jdvmlinuxusr jenkins[7110]: 2023-04-08 05:57:10.928+0000 [id=46]        INFO        h.m.DownloadService$Downloadable#load: Obtained the updated data file for hudson.tasks.Maven.MavenInstaller
Apr 08 11:27:10 jdvmlinuxusr jenkins[7110]: 2023-04-08 05:57:10.930+0000 [id=46]        INFO        hudson.util.Retrier#start: Performed the action check updates server successfully at the attempt #1
jdvmlinuxusr@jdvmlinuxusr:~$ sudo cat /var/lib/jenkins/secrets/
[sudo] password for jdvmlinuxusr:
Sorry, try again.
[sudo] password for jdvmlinuxusr:
cat: /var/lib/jenkins/secrets/: Is a directory
jdvmlinuxusr@jdvmlinuxusr:~$ cd /var/
jdvmlinuxusr@jdvmlinuxusr:/var$ pwd
/var
jdvmlinuxusr@jdvmlinuxusr:/var$ ls
backups  cache  crash  lib  local  lock  log  mail  metrics  opt  run  snap  spool  tmp
jdvmlinuxusr@jdvmlinuxusr:/var$ cd lib/
jdvmlinuxusr@jdvmlinuxusr:/var/lib$ ls
AccountsService  aspell         command-not-found    emacsen-common  hp           man-db          pam                    saned         sudo              ubuntu-drivers-common    update-notifier  xfonts
acpi-support     avahi-autoipd  dbus                 fprint          ispell       misc            plymouth               sgml-base     swcatalog         ubuntu-release-upgrader  upower           xkb
alsa             bluetooth      dhcp                 gdm3            jenkins      NetworkManager  polkit-1               shells.state  systemd           ucf                      usb_modeswitch   xml-core
app-info         boltd          dictionaries-common  geoclue         libreoffice  openvpn         power-profiles-daemon  shim-signed   tpm               udisks2                  usbutils
apport           BrlAPI         dkms                 ghostscript     locales      os-prober       private                snapd         ubiquity          unattended-upgrades      vim
apt              colord         dpkg                 grub            logrotate    PackageKit      python                 snmp          ubuntu-advantage  update-manager           whoopsie
jdvmlinuxusr@jdvmlinuxusr:/var/lib$ cd jenkins/
jdvmlinuxusr@jdvmlinuxusr:/var/lib/jenkins$ ls
config.xml  hudson.model.UpdateCenter.xml  jenkins.telemetry.Correlator.xml  jobs  nodeMonitors.xml  nodes  plugins  secret.key  secret.key.not-so-secret  secrets  updates  userContent  users
jdvmlinuxusr@jdvmlinuxusr:/var/lib/jenkins$ cd secrets/
-bash: cd: secrets/: Permission denied
jdvmlinuxusr@jdvmlinuxusr:/var/lib/jenkins$ ls
config.xml  hudson.model.UpdateCenter.xml  jenkins.telemetry.Correlator.xml  jobs  nodeMonitors.xml  nodes  plugins  secret.key  secret.key.not-so-secret  secrets  updates  userContent  users
jdvmlinuxusr@jdvmlinuxusr:/var/lib/jenkins$ sudo cd secrets/
sudo: cd: command not found
sudo: "cd" is a shell built-in command, it cannot be run directly.
sudo: the -s option may be used to run a privileged shell.
sudo: the -D option may be used to run a command in a specific directory.
jdvmlinuxusr@jdvmlinuxusr:/var/lib/jenkins$ cd secrets/
-bash: cd: secrets/: Permission denied
jdvmlinuxusr@jdvmlinuxusr:/var/lib/jenkins$ sudo -i
root@jdvmlinuxusr:~# pws
Command 'pws' not found, did you mean:
  command 'aws' from snap aws-cli (1.15.58)
  command 'psw' from deb wise (2.4.1-23)
  command 'pts' from deb openafs-client (1.8.8.1-3ubuntu2~22.04.1)
  command 'pvs' from deb lvm2 (2.03.11-2.1ubuntu4)
  command 'ps' from deb procps (2:3.3.17-6ubuntu2)
  command 'aws' from deb awscli (1.22.34-1)
  command 'pcs' from deb pcs (0.10.11-2ubuntu3)
  command 'pms' from deb pms (0.42-1build4)
  command 'pwd' from deb coreutils (8.32-4.1ubuntu1)
  command 'pps' from deb libpmix-bin (4.1.2-2ubuntu1)
  command 'rpws' from deb ratpoison (1.4.9-1)
See 'snap info <snapname>' for additional versions.
root@jdvmlinuxusr:~# pwd
/root
root@jdvmlinuxusr:~# cd /var/lib/jenkins/secrets/
root@jdvmlinuxusr:/var/lib/jenkins/secrets# ls
initialAdminPassword  jenkins.model.Jenkins.crumbSalt  master.key
root@jdvmlinuxusr:/var/lib/jenkins/secrets# cat initialAdminPassword
5ac5938db28c40e4bac40ca2c08cbc38
root@jdvmlinuxusr:/var/lib/jenkins/secrets# ^C
root@jdvmlinuxusr:/var/lib/jenkins/secrets#

```
### Jenkins Admin User Details
- usr/pass : jdjenkinusr
```bash
jdvmlinuxusr@jdvmlinuxusr:~$ wget http://192.168.1.10:8080/jnlpJars/jenkins-cli.jar
jdvmlinuxusr@jdvmlinuxusr:~$ java -jar jenkins-cli.jar -s http://192.168.1.10:8080/ -auth jdjenkinusr:112aec9977e3ac1eeba8d81352af40abcf


jdvmlinuxusr@jdvmlinuxusr:~$ java -jar jenkins-cli.jar -s http://192.168.1.10:8080/ -auth jdjenkinusr:112aec9977e3ac1eeba8d81352af40abcf -webSocket list-jobs
jdvmlinuxusr@jdvmlinuxusr:~$ java -jar jenkins-cli.jar -s http://192.168.1.10:8080/ -auth jdjenkinusr:112aec9977e3ac1eeba8d81352af40abcf -webSocket list-jobs
test2
jdvmlinuxusr@jdvmlinuxusr:~$ java -jar jenkins-cli.jar -s http://192.168.1.10:8080/ -auth jdjenkinusr:112aec9977e3ac1eeba8d81352af40abcf -webSocket build test2
jdvmlinuxusr@jdvmlinuxusr:~$


````
### Plugins
![image](https://user-images.githubusercontent.com/69948118/230713957-ad438c44-dad7-4c8f-b12f-28d5051dcf01.png)

`sudo systemctl restart jenkins`

## Jekin Admin
![image](https://user-images.githubusercontent.com/69948118/230714200-358c7fc7-2996-43e1-8b8d-26c72c1d3187.png)
![image](https://user-images.githubusercontent.com/69948118/230714246-5b0c00b9-b487-40e6-b15c-1bf4115361f4.png)
![image](https://user-images.githubusercontent.com/69948118/230714306-012a142b-3ecf-4c02-a9bc-2ad12b17f134.png)

```

jdvmlinuxusr@jdvmlinuxusr:~$ pwd
/home/jdvmlinuxusr
jdvmlinuxusr@jdvmlinuxusr:~$ mkdir jenkinsbakcup
jdvmlinuxusr@jdvmlinuxusr:~$ cd jenkinsbakcup/
jdvmlinuxusr@jdvmlinuxusr:~/jenkinsbakcup$ pwd
/home/jdvmlinuxusr/jenkinsbakcup
jdvmlinuxusr@jdvmlinuxusr:~/jenkinsbakcup$ chmod 777 jenkinsbakcup
chmod: cannot access 'jenkinsbakcup': No such file or directory
jdvmlinuxusr@jdvmlinuxusr:~/jenkinsbakcup$ cd ..
jdvmlinuxusr@jdvmlinuxusr:~$ chmod 777 jenkinsbakcup/
jdvmlinuxusr@jdvmlinuxusr:~$

```

## Piplines
![image](https://user-images.githubusercontent.com/69948118/230715837-7cf48fdd-a977-4887-8f33-0c84fead85c3.png)
![image](https://user-images.githubusercontent.com/69948118/230715939-5a36d162-88b3-4193-a8d6-49b35f76e44c.png)
![image](https://user-images.githubusercontent.com/69948118/230715955-05d5929c-bf27-4cb1-bc03-fbb7a583651d.png)
![image](https://user-images.githubusercontent.com/69948118/230716230-0779c363-ccb1-4273-949d-462e1dd4235d.png)
![image](https://user-images.githubusercontent.com/69948118/230716179-d879fd85-2fa1-4dea-bc46-4be4822c94eb.png)


## Docker Overview
![image](https://user-images.githubusercontent.com/69948118/230749666-5d9fd4f5-1805-4a0e-9227-0358b5e3aeff.png)
![image](https://user-images.githubusercontent.com/69948118/230749684-1c972447-157b-4e8a-98f7-1c87a538c2f2.png)
![image](https://user-images.githubusercontent.com/69948118/230749706-4e056a18-7304-4965-981d-e4e8023706b5.png)
![image](https://user-images.githubusercontent.com/69948118/230749775-4a4396ac-842f-4fe0-bb8f-cd21c057724e.png)
![image](https://user-images.githubusercontent.com/69948118/230749794-553783bd-b5a9-4efd-a3b3-e2c955a38fda.png)
![image](https://user-images.githubusercontent.com/69948118/230749831-7e9bb38f-757f-4cdd-b00a-49c3460c26c1.png)
![image](https://user-images.githubusercontent.com/69948118/230749859-b4701939-9088-43b2-9654-ab1f1c48f1a6.png)

## Docker install
```
 curl -fsSL https://get.docker.com -o get-docker.sh
 sudo sh get-docker.sh
 
 ```
 ## Docker commands
![image](https://user-images.githubusercontent.com/69948118/230750261-ec5643eb-95b5-4434-aeb2-b2c5ca3e76ed.png)
![image](https://user-images.githubusercontent.com/69948118/230750270-dfb8010a-3b7e-4424-8331-a94ff961534f.png)
![image](https://user-images.githubusercontent.com/69948118/230750287-46afa1ff-3b72-4c46-b737-9ff16bafd454.png)
![image](https://user-images.githubusercontent.com/69948118/230750306-36e3c041-9bf9-44b5-88db-2cff899a56fc.png)
![image](https://user-images.githubusercontent.com/69948118/230750321-a8098096-9faf-4292-a0a5-c6617a5b4d8b.png)
![image](https://user-images.githubusercontent.com/69948118/230750339-80b5d339-0fc2-4b03-9a4d-1b13e864aeba.png)
![image](https://user-images.githubusercontent.com/69948118/230750345-14f3c267-f780-4a57-8e40-a8973fcb1bd9.png)
![image](https://user-images.githubusercontent.com/69948118/230750356-ae692d06-06dd-426b-8801-9f127d95aeb4.png)
![image](https://user-images.githubusercontent.com/69948118/230750427-58c42ca3-1c4d-4a99-902b-78e4d3a90d92.png)
![image](https://user-images.githubusercontent.com/69948118/230750472-7f79a639-ba74-4f8d-8dc2-b7aaa3954760.png)

## Docker Run
![image](https://user-images.githubusercontent.com/69948118/230753033-6e1d1367-7454-42a2-93db-1a855e7292c3.png)
![image](https://user-images.githubusercontent.com/69948118/230753099-03f17537-d90f-4b6a-a0dc-f449fae8c0f9.png)
![image](https://user-images.githubusercontent.com/69948118/230753216-7dd40307-e39c-47da-bbd7-fdd87a636271.png)
![image](https://user-images.githubusercontent.com/69948118/230753277-10b5b05a-21fe-4f5a-8444-46871df08b02.png)
![image](https://user-images.githubusercontent.com/69948118/230753291-05aab625-4803-4dd1-9b2f-15f79578cf51.png)
![image](https://user-images.githubusercontent.com/69948118/230753307-2790b735-6e68-4631-8943-4cc4c4b064c1.png)
![image](https://user-images.githubusercontent.com/69948118/230753492-58a9d11d-7593-4891-9bfa-c20f6d6669a1.png)
![image](https://user-images.githubusercontent.com/69948118/230753592-6a3d452d-5fa6-4218-8820-b2658bc986f6.png)
![image](https://user-images.githubusercontent.com/69948118/230753650-cd638216-648a-443a-9e25-69600e20bddf.png)

## Docker Images
![image](https://user-images.githubusercontent.com/69948118/230754285-f93b0f5f-95b9-4913-9768-83ffac9c6d91.png)
![image](https://user-images.githubusercontent.com/69948118/230754318-b1636051-af2f-4e6f-abf8-647a6fecebe2.png)
![image](https://user-images.githubusercontent.com/69948118/230754339-f06d22bd-33da-4202-a07a-98ad5b48b5c4.png)
![image](https://user-images.githubusercontent.com/69948118/230754381-2b7cd5c0-6c40-40e2-8e58-0a808113e96e.png)
![image](https://user-images.githubusercontent.com/69948118/230754388-f4a9aae8-6999-44ea-8d9b-1801ba0ad00f.png)
![image](https://user-images.githubusercontent.com/69948118/230754404-e8e2e772-7b01-40ac-817d-280fa0b6fc86.png)
![image](https://user-images.githubusercontent.com/69948118/230754427-72167b8d-4d38-46d3-bb3a-aaf5e11114ff.png)

## Environment Varilables
![image](https://user-images.githubusercontent.com/69948118/230759550-0385c4dc-8223-4b89-bd60-aa8361cb0afe.png)
![image](https://user-images.githubusercontent.com/69948118/230759565-9f6f5a21-cb04-4c33-ad3e-9eae5c0a08cf.png)
![image](https://user-images.githubusercontent.com/69948118/230759573-56b3097b-8d79-4ef3-9a61-d62fa37ca7a2.png)
![image](https://user-images.githubusercontent.com/69948118/230759588-4ccfabab-cc80-44ec-92b6-7c4956f5bbfc.png)
```
$ docker run -p 38282:8080 --name blue-app -e APP_COLOR=blue -d kodekloud/simple-webapp
282d668b854138948001a056a133760e8cb3d6a1c557b971d0d18d2ff72f9ffa
```
## Commands vs Entypoint
![image](https://user-images.githubusercontent.com/69948118/230760077-7e98019c-02dc-4539-ba62-818581a45a87.png)
![image](https://user-images.githubusercontent.com/69948118/230760090-fdcf420b-6435-429c-bae5-41b673f04d51.png)
- CMD from image will be override if we will provide the CMD during docker run 
![image](https://user-images.githubusercontent.com/69948118/230760123-295afb97-d5ed-4ce0-9b25-77aa15683ec1.png)
![image](https://user-images.githubusercontent.com/69948118/230760155-38462d8b-4651-49ab-ae74-cf23b0b128fb.png)
- In case of Entrypoint command will be appended which we pass during docker run 
![image](https://user-images.githubusercontent.com/69948118/230760189-d3fd3aec-7f84-4005-bee6-59bf4f749e45.png)
![image](https://user-images.githubusercontent.com/69948118/230760308-58ced740-58df-4ef1-a52c-4330b559077c.png)

 ## Docker Engine_Storage and Networking
 ![image](https://user-images.githubusercontent.com/69948118/230760541-fbab46d3-6d57-4a4f-bbef-a282368c03d9.png)
![image](https://user-images.githubusercontent.com/69948118/230760559-5226734d-d4e6-4507-abf3-9d98c5e5399a.png)
![image](https://user-images.githubusercontent.com/69948118/230760647-7965988c-d977-477f-8bd9-037b9a60bdd1.png)
![image](https://user-images.githubusercontent.com/69948118/230760711-3c46607f-a1ed-4ac8-b998-6913e7555e6d.png)
### Storage
![image](https://user-images.githubusercontent.com/69948118/230760790-ab86e771-baf9-40fc-bedc-35d2b1576fee.png)
![image](https://user-images.githubusercontent.com/69948118/230760933-bd87919d-a4d1-4650-af39-6ead4ec7b15e.png)
![image](https://user-images.githubusercontent.com/69948118/230761037-04923b4e-133d-4357-adc1-0eb80bb84e30.png)
![image](https://user-images.githubusercontent.com/69948118/230761125-0b785c29-5d5f-42da-a3e1-b90975515555.png)
![image](https://user-images.githubusercontent.com/69948118/230761247-4f3a4ae8-1886-4d45-b6ec-d6cf34da8374.png)
![image](https://user-images.githubusercontent.com/69948118/230761280-637b4672-855d-4d41-a243-f7b637ffcfa9.png)
![image](https://user-images.githubusercontent.com/69948118/230761321-ee17f099-178f-4a52-a938-e658d96678ea.png)

### Networking
![image](https://user-images.githubusercontent.com/69948118/230761738-5ffb5ac3-99e6-4323-8d6e-3dceaa4a5d72.png)
![image](https://user-images.githubusercontent.com/69948118/230761772-6fb747bf-7175-4731-99bd-a36d26c0a4cf.png)
![image](https://user-images.githubusercontent.com/69948118/230761789-078914c4-190b-4a4f-b07e-36a69944b891.png)
![image](https://user-images.githubusercontent.com/69948118/230761833-a96f4888-eb1c-430b-ae57-323ec63ed8ad.png)
```
Deploy a web application named webapp using the kodekloud/simple-webapp-mysql image. Expose the port to 38080 on the host.

The application makes use of two environment variable:
1: DB_Host with the value mysql-db.
2: DB_Password with the value db_pass123.
Make sure to attach it to the newly created network called wp-mysql-network.

Also make sure to link the MySQL and the webapp container.
```
```
docker run --network=wp-mysql-network -e DB_Host=mysql-db -e DB_Password=db_pass123 -p 38080:8080 --name webapp --link mysql-db:mysql-db -d kodekloud/simple-webapp-mysql
```

## Docker Registry
![image](https://user-images.githubusercontent.com/69948118/230762306-51c171d8-f2d4-4b45-8624-1d0ea632475a.png)
![image](https://user-images.githubusercontent.com/69948118/230762353-c3508b28-7de9-4d24-a7e8-b96c4941799d.png)
![image](https://user-images.githubusercontent.com/69948118/230762417-bc98bcb5-c108-44f5-b2f0-01234401ea19.png)


## Kubernetes Overview
![image](https://user-images.githubusercontent.com/69948118/230764405-4def7ef8-982b-423d-bcf9-3faa6a916841.png)
![image](https://user-images.githubusercontent.com/69948118/230764517-a97932a6-62ff-4c78-afb5-c232be55b12d.png)
![image](https://user-images.githubusercontent.com/69948118/230764532-3800c4dc-c045-42cc-b416-9d0a71f34f05.png)
![image](https://user-images.githubusercontent.com/69948118/230764613-3ef09197-c06f-41f5-82b4-43b2134f574c.png)
![image](https://user-images.githubusercontent.com/69948118/230764669-5e11ddb8-8183-4d40-abe0-1d8088a5b414.png)
![image](https://user-images.githubusercontent.com/69948118/230764705-54c6cc16-8be1-45a4-933f-9978d515f3b5.png)
![image](https://user-images.githubusercontent.com/69948118/230764719-015498b6-15c0-4d58-9822-2e8f13beb061.png)
![image](https://user-images.githubusercontent.com/69948118/230764739-0f58ada1-dcfb-49e3-baf8-059a96463bd1.png)
![image](https://user-images.githubusercontent.com/69948118/230764816-b8b02cfb-fc0a-44cb-baa7-1838bcc71796.png)
![image](https://user-images.githubusercontent.com/69948118/230764877-35948064-bf4c-4701-a21d-6b06fc055512.png)
![image](https://user-images.githubusercontent.com/69948118/230765574-8bdfc620-31ad-4775-bf43-79d838732647.png)

## Setup Kubernetes
![image](https://user-images.githubusercontent.com/69948118/230765640-55453682-8f7e-4197-920e-ffa6079d349b.png)
![image](https://user-images.githubusercontent.com/69948118/230765709-c257b52d-1dfb-4c32-a978-2615ad6bf257.png)
![image](https://user-images.githubusercontent.com/69948118/230765749-7ef2cc8b-97db-4b2c-bfe3-61caee239a2c.png)
### Install kubectl binary with curl on Linux 
```bash
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
chmod +x kubectl
mv ./kubectl user/local/bin/kubectl
```
```
Install and set up the kubectl tool: –

https://kubernetes.io/docs/tasks/tools/

Install Minikube: –

https://minikube.sigs.k8s.io/docs/start/

Install VirtualBox: –

https://www.virtualbox.org/wiki/Downloads

https://www.virtualbox.org/wiki/Linux_Downloads

Minikube Tutorial: –

https://kubernetes.io/docs/tutorials/hello-minikube/

If the minikube installation has been done on the macOS, then to access the URL on the local browser, we need to do a few steps to get the service URL to work. Those steps are covered on this documentation page: –

https://minikube.sigs.k8s.io/docs/handbook/accessing/#using-minikube-service-with-tunnel
```

## Kubernetes COncept
### PODS
![image](https://user-images.githubusercontent.com/69948118/230807554-81ff93c1-ffa6-4855-ac23-22a9260ce93d.png)
![image](https://user-images.githubusercontent.com/69948118/230807622-c124f9d9-da75-43a7-a52e-d56f776069d6.png)
![image](https://user-images.githubusercontent.com/69948118/230807734-14eec78d-cadf-4ea2-9ae1-9c93b74c0b69.png)
![image](https://user-images.githubusercontent.com/69948118/230807777-1072e840-41b6-49ae-8b01-0f496e36d916.png)
![image](https://user-images.githubusercontent.com/69948118/230807951-7c3123df-5fb3-48ef-b37e-d9478370ce21.png)
![image](https://user-images.githubusercontent.com/69948118/230808160-f721a687-92c7-4b4c-99b7-e7fa7bf32040.png)
![image](https://user-images.githubusercontent.com/69948118/230808206-be26ce98-e7f9-4015-972a-b87bf52f910d.png)
![image](https://user-images.githubusercontent.com/69948118/230808379-42d7719f-64bd-48d1-89ac-afbb20c6c693.png)

### YAML
![image](https://user-images.githubusercontent.com/69948118/230809100-8ad4b44f-e668-4d84-8c3b-55ed6386438d.png)
![image](https://user-images.githubusercontent.com/69948118/230809201-3106cd89-7807-4ca9-9071-9fa212e29b38.png)
![image](https://user-images.githubusercontent.com/69948118/230809348-b7490867-677d-4b0f-87b9-14e988d28746.png)
![image](https://user-images.githubusercontent.com/69948118/230809394-1b57947e-016b-4eab-ac2f-93bca9dfe383.png)
![image](https://user-images.githubusercontent.com/69948118/230809456-6eae20e7-4e17-4569-9901-52e76bbe803b.png)
![image](https://user-images.githubusercontent.com/69948118/230809575-8f8870f8-6809-4109-9f45-c543873c495b.png)

## Pods, Replicaset, Deployments
![image](https://user-images.githubusercontent.com/69948118/230811304-ad40e68c-cacb-4d74-9779-11ced3983f93.png)
![image](https://user-images.githubusercontent.com/69948118/230811338-50778d35-6ee0-4d1a-8159-4c6f86530014.png)
![image](https://user-images.githubusercontent.com/69948118/230811388-e164946d-8c35-47c8-9e01-9e2fa6d512f2.png)
![image](https://user-images.githubusercontent.com/69948118/230811801-114e8fff-1296-470d-80fb-3dad1c64dfc4.png)
### yaml ide
- VS code
- Plugin
 ![image](https://user-images.githubusercontent.com/69948118/230812539-3152b2d5-363a-4b90-93aa-2eb85f492042.png)
- VS code setting
![image](https://user-images.githubusercontent.com/69948118/230812880-91928b4e-ae18-4f92-afb7-0a8ee1629d3d.png)

```
controlplane ~ ➜  kubectl run nginx --image=nginx
pod/nginx created

controlplane ~ ➜  kubectl get pods
NAME    READY   STATUS              RESTARTS   AGE
nginx   0/1     ContainerCreating   0          9s

controlplane ~ ➜  kubectl describe pod newpods-jjbmc
controlplane ~ ➜  kubectl delete pod webapp 
controlplane ~ ➜  kubectl run redis --image=redis123 --dry-run=client -o yaml > redis-definition.yaml
controlplane ~ ➜  kubectl create -f redis-definition.yaml 
```
## Controller
![image](https://user-images.githubusercontent.com/69948118/230827376-e1f87aa8-104d-4e92-aed6-2813eb3a8a7f.png)
![image](https://user-images.githubusercontent.com/69948118/230827479-7854f5da-857b-4dcf-b7e6-195e1ba669a0.png)
- Replication controller vs ReplicaSet
![image](https://user-images.githubusercontent.com/69948118/230827980-23e3d03b-7b1f-4466-9f2c-bc8f1472bd93.png)
![image](https://user-images.githubusercontent.com/69948118/230828368-5956d533-5bf0-4ab4-88cf-62d4d20d23f3.png)
![image](https://user-images.githubusercontent.com/69948118/230828511-08a59942-9e6f-411f-991a-fe47cbafc433.png)
![image](https://user-images.githubusercontent.com/69948118/230828793-5f07d2cb-e0cd-41e4-b85a-5ec00d33f019.png)
![image](https://user-images.githubusercontent.com/69948118/230828878-9ad85176-9e3d-4599-b5ae-a581f7ba6433.png)
![image](https://user-images.githubusercontent.com/69948118/230830112-7f8d20f1-4845-4102-8448-246cc9150b5b.png)
### Deployment
![image](https://user-images.githubusercontent.com/69948118/231031209-8ee751f3-f527-4bef-860f-b18df4b2263e.png)
![image](https://user-images.githubusercontent.com/69948118/231031356-a1144de9-af2b-494e-ae09-a696c6d6f93d.png)
![image](https://user-images.githubusercontent.com/69948118/231031450-dbf65431-339f-4baf-8d28-1f9251920dae.png)

### Updated and Rollback
![image](https://user-images.githubusercontent.com/69948118/231033829-c5770e06-087a-4f84-b5fa-6d89307f49de.png)
![image](https://user-images.githubusercontent.com/69948118/231033928-f3842c2f-7bc1-41fe-a44f-84f1a6b524e6.png)
![image](https://user-images.githubusercontent.com/69948118/231034098-e1d70bfe-cd40-4885-995c-c723803dd4ad.png)
![image](https://user-images.githubusercontent.com/69948118/231034248-38e9338e-8891-43aa-afac-808e053399b1.png)
![image](https://user-images.githubusercontent.com/69948118/231034378-80c78177-91fa-4c74-93c2-cf9d254f0cc3.png)
![image](https://user-images.githubusercontent.com/69948118/231034518-c6e22cad-0ec7-447b-8100-13d902ecd0b6.png)
![image](https://user-images.githubusercontent.com/69948118/231034678-e0cf1ff9-ddc4-4f93-b114-9721fa42095b.png)
![image](https://user-images.githubusercontent.com/69948118/231034774-fed20ad1-4a46-4a65-ac2e-e695cb4ae02c.png)
![image](https://user-images.githubusercontent.com/69948118/231034937-e6802c96-a70b-414c-be0e-265df6004895.png)
![image](https://user-images.githubusercontent.com/69948118/231035580-027bf9e8-7132-4b3c-865e-65602921ccc2.png)
![image](https://user-images.githubusercontent.com/69948118/231036299-85ebd683-5320-4aa3-ac18-a0665bbd1fe5.png)
![image](https://user-images.githubusercontent.com/69948118/231036448-f840f359-f665-415a-b85c-b4452eebe120.png)

## Netwroking in kubernetes
![image](https://user-images.githubusercontent.com/69948118/231037134-94b721e2-a73d-4613-a26b-65b8535cc68a.png)
![image](https://user-images.githubusercontent.com/69948118/231037346-ccb10745-9d95-43f7-93c0-738ff6ec789b.png)
![image](https://user-images.githubusercontent.com/69948118/231037503-38bf0256-beb2-416a-b68e-4f2500c6b6d7.png)
![image](https://user-images.githubusercontent.com/69948118/231037627-9fd4c04e-b71c-4c91-af3c-9d57357f314c.png)
![image](https://user-images.githubusercontent.com/69948118/231037864-c1f98255-25c0-46d5-9521-c2482553b793.png)
## Services in kubernetes
![image](https://user-images.githubusercontent.com/69948118/231038106-98ad0a62-e48f-470e-97ee-fc3bae7c751d.png)
![image](https://user-images.githubusercontent.com/69948118/231038390-d103a2eb-5af1-42a6-807b-f28b908bd374.png)
![image](https://user-images.githubusercontent.com/69948118/231038448-fc99a320-3a70-43fc-82ab-fafa9c6b7113.png)
![image](https://user-images.githubusercontent.com/69948118/231038548-f1496b3d-546d-45c8-8b59-67e12f6a23e4.png)
![image](https://user-images.githubusercontent.com/69948118/231038647-92e28ada-19fb-4bd4-843b-84689b6aca5a.png)
![image](https://user-images.githubusercontent.com/69948118/231038866-c09825f8-9eec-4e50-a36b-edca1765eec2.png)
![image](https://user-images.githubusercontent.com/69948118/231039067-118ae499-6623-4338-9d55-e774006aad58.png)
![image](https://user-images.githubusercontent.com/69948118/231039707-aa798ac9-2240-41a5-8dfa-ccf4b5bb4a06.png)
![image](https://user-images.githubusercontent.com/69948118/231039793-7bd808b5-5d94-4588-bb00-4b6dfa9a0f33.png)
![image](https://user-images.githubusercontent.com/69948118/231039897-b76aa102-0a39-4921-986d-a50668285a3b.png)
![image](https://user-images.githubusercontent.com/69948118/231040034-65d8a9e3-343c-46c0-ab9c-078a81416d2c.png)
![image](https://user-images.githubusercontent.com/69948118/231040859-745b7f16-f1bf-4804-b1c7-28b53b750058.png)
![image](https://user-images.githubusercontent.com/69948118/231041281-e156ba03-c59a-4a29-833f-457129592dcd.png)
![image](https://user-images.githubusercontent.com/69948118/231041585-6ef19f1d-b8a5-4201-a358-623b2ebea303.png)
![image](https://user-images.githubusercontent.com/69948118/231042012-15d9a33e-ac6b-4fe4-8474-bed16ca5e29a.png)
![image](https://user-images.githubusercontent.com/69948118/231042124-72a97f4f-e60f-4ab8-929a-5818897f973e.png)

## Microservices Architecture
![image](https://user-images.githubusercontent.com/69948118/231052851-cb612d25-0d05-4c9e-bdd2-89f946999a68.png)
![image](https://user-images.githubusercontent.com/69948118/231053111-4f2497fe-cca8-4fee-b7b1-d8efe74b8fe2.png)
![image](https://user-images.githubusercontent.com/69948118/231053260-f7e13c14-f1b5-4c59-91d9-39578ad26ebd.png)
![image](https://user-images.githubusercontent.com/69948118/231053302-6152e482-74e1-4978-855f-c85efa844d66.png)
![image](https://user-images.githubusercontent.com/69948118/231053386-43fb4ad1-19b9-44f1-a345-3589c14c5756.png)
![image](https://user-images.githubusercontent.com/69948118/231053405-ae59dc18-c797-4a00-974f-73a4dc65f837.png)
![image](https://user-images.githubusercontent.com/69948118/231053456-95d8233a-0dad-487f-bfc3-5e2d51156f5b.png)
![image](https://user-images.githubusercontent.com/69948118/231053617-a683add0-e62a-4491-86f4-90e663dd2d53.png)
![image](https://user-images.githubusercontent.com/69948118/231053790-ef76f7ae-2a5d-4a69-b04d-9a434f5bb7ef.png)
![image](https://user-images.githubusercontent.com/69948118/231054054-a0f4a385-fd5a-4e22-8a4d-46e217a5fd3a.png)
![image](https://user-images.githubusercontent.com/69948118/231054168-02970bdf-201b-4577-a38c-c3fe5f0e5bca.png)
![image](https://user-images.githubusercontent.com/69948118/231054278-6e40c74e-a25d-429a-9ef0-9a9d4612e0f7.png)
![image](https://user-images.githubusercontent.com/69948118/231054416-463d2475-093f-4383-8fd6-2bd952038b64.png)
![image](https://user-images.githubusercontent.com/69948118/231057492-c460429f-6963-4140-b1e5-cfb6befab8ee.png)

## Ansible Intro
![image](https://user-images.githubusercontent.com/69948118/231064077-8b2d801b-6f78-4847-b2af-fc69c9e9ac1b.png)
![image](https://user-images.githubusercontent.com/69948118/231064168-9f98cb97-d479-4363-b503-d7cad3f6f581.png)
![image](https://user-images.githubusercontent.com/69948118/231064207-210ac753-a31d-4c88-85af-599c1ba3f814.png)
![image](https://user-images.githubusercontent.com/69948118/231064435-1cb00f35-1239-46b2-bdc6-cc99f1bd4596.png)

## Setup
- Download the VDI from osboxres
- https://www.osboxes.org/debian/#debian-11-vbox
- create three different virtual machine controller , ansible targe1 and target2
![image](https://user-images.githubusercontent.com/69948118/231098331-338433f0-2d03-4f49-a660-623d4b1a677e.png)
![image](https://user-images.githubusercontent.com/69948118/231098581-884b0d57-3262-4873-8ec1-6284a512e346.png)
![image](https://user-images.githubusercontent.com/69948118/231099949-b1e79d88-30b0-4d0a-a5fe-9478bd3670fd.png)

## Ansible Concpet
### Inventory
![image](https://user-images.githubusercontent.com/69948118/231101397-c8d20b6d-efca-4b48-96a8-843b2c7b170a.png)
![image](https://user-images.githubusercontent.com/69948118/231101488-a50c4487-1ca9-4223-92da-c39fb9595eb7.png)
![image](https://user-images.githubusercontent.com/69948118/231101576-0e7cb716-9cfe-40c6-bf2d-d547f310d95b.png)
![image](https://user-images.githubusercontent.com/69948118/231102159-853bd6d0-e357-4c7b-8cec-10775f6edd45.png)

### Playbooks
![image](https://user-images.githubusercontent.com/69948118/231104919-c3c4d438-0b34-44c6-bf12-10f05ca72dfb.png)
![image](https://user-images.githubusercontent.com/69948118/231105324-d8f39b35-657b-4909-8097-9aca55a50b78.png)
![image](https://user-images.githubusercontent.com/69948118/231105695-612c5817-126f-4e04-90a4-bb181a318239.png)
![image](https://user-images.githubusercontent.com/69948118/231105814-fce236bf-1001-4dd0-bac9-e5682364a68c.png)
![image](https://user-images.githubusercontent.com/69948118/231106077-206b39de-5398-4d10-b7dd-4961f0620549.png)
![image](https://user-images.githubusercontent.com/69948118/231106285-5655c007-c99a-4ffa-a6f5-a5d4b912988e.png)
### Modules
![image](https://user-images.githubusercontent.com/69948118/231119252-3f110672-12d2-4ef6-98da-d3b52de0c287.png)
![image](https://user-images.githubusercontent.com/69948118/231119349-f8effca3-edcf-462c-85cf-cb41af31ccfa.png)
![image](https://user-images.githubusercontent.com/69948118/231119444-ab6fa7ce-e218-417f-9e9d-a9b566d34eb8.png)
![image](https://user-images.githubusercontent.com/69948118/231119540-d87d5347-37ec-40ce-9f59-3f09484a1301.png)
![image](https://user-images.githubusercontent.com/69948118/231119626-31cd42a3-6a07-4d90-b4ce-24d240965b33.png)
![image](https://user-images.githubusercontent.com/69948118/231119768-5b00a290-179a-4fde-ae8e-2b6c4a7f1412.png)
![image](https://user-images.githubusercontent.com/69948118/231120402-f0d6a654-ef23-460d-b150-bdb41b15fd4f.png)
![image](https://user-images.githubusercontent.com/69948118/231120689-42300147-2f00-4c24-9683-f84cd1225d04.png)
![image](https://user-images.githubusercontent.com/69948118/231120954-0394dff7-5b98-45bb-a20c-929ccd6e4ef2.png)
![image](https://user-images.githubusercontent.com/69948118/231121260-a770d986-c3ca-462a-91e4-a5da26aee84e.png)
![image](https://user-images.githubusercontent.com/69948118/231121602-7c51f35e-bef5-4181-8e2d-5d1fc5ecdedc.png)
![image](https://user-images.githubusercontent.com/69948118/231122000-6b78df03-21d9-410e-8e68-8b51e1ba6e10.png)
### Variables
![image](https://user-images.githubusercontent.com/69948118/231125817-adb9926e-8c51-458d-a4e0-77435485c76f.png)
![image](https://user-images.githubusercontent.com/69948118/231126127-68a76573-abe4-475b-bc2d-e80871fb61a2.png)
![image](https://user-images.githubusercontent.com/69948118/231126459-8f3b6181-25f8-4bd9-8e23-28fde028fc89.png)
![image](https://user-images.githubusercontent.com/69948118/231126672-2138afb2-fb4a-42b1-a378-eac0c20e1a87.png)
### Ansible Conditionals
![image](https://user-images.githubusercontent.com/69948118/231128059-17e9ded6-84cf-4de6-b7a6-6575733ac824.png)
![image](https://user-images.githubusercontent.com/69948118/231128179-561617b4-6960-4616-96df-8cd4f8523817.png)
![image](https://user-images.githubusercontent.com/69948118/231128474-f50ab3be-ab59-44a2-9983-72f077437523.png)
![image](https://user-images.githubusercontent.com/69948118/231128516-928812e9-cb5d-42fd-b667-6cb9d19e3d1b.png)
![image](https://user-images.githubusercontent.com/69948118/231128676-963465af-0aac-4844-a5df-7a5495a57ecd.png)
### Anisble loops
![image](https://user-images.githubusercontent.com/69948118/231130443-9bcf57eb-3122-444a-9d26-8a7cd2c10c7f.png)
![image](https://user-images.githubusercontent.com/69948118/231130635-45b47046-a5f1-4bf9-ad4f-8182c2974f37.png)
![image](https://user-images.githubusercontent.com/69948118/231131200-f457468b-3b1e-4712-8d21-6e7e52dc07d9.png)
![image](https://user-images.githubusercontent.com/69948118/231131357-a0e50c60-bd79-4f87-b95c-b2de18482ca7.png)
![image](https://user-images.githubusercontent.com/69948118/231131442-dc443cff-b665-4905-be60-42b2e5e7e176.png)
![image](https://user-images.githubusercontent.com/69948118/231131631-124a4468-ff06-4625-9f0e-a73a09e6e006.png)
![image](https://user-images.githubusercontent.com/69948118/231131684-3132f254-e715-4ab5-9b49-0e4387146ca1.png)
### Ansible Roles
![image](https://user-images.githubusercontent.com/69948118/231132639-5f4ac891-1538-487a-af33-94244ba3df8a.png)
![image](https://user-images.githubusercontent.com/69948118/231132844-0ffbd18b-fba9-463e-9881-c3c0f206e2f7.png)
![image](https://user-images.githubusercontent.com/69948118/231133120-3428acf9-fc6b-4e33-b85f-9d653d75f108.png)
![image](https://user-images.githubusercontent.com/69948118/231133264-5f060576-1421-49bd-9bb1-6fd7bf86a4db.png)
![image](https://user-images.githubusercontent.com/69948118/231133312-2803a0f5-5325-4127-b9e5-781d162862fb.png)
![image](https://user-images.githubusercontent.com/69948118/231133741-e61641b6-cb74-4c1f-97f7-a202b9ea2f19.png)
![image](https://user-images.githubusercontent.com/69948118/231133900-be85598b-d652-4ef0-a012-c5039678bd95.png)
![image](https://user-images.githubusercontent.com/69948118/231133981-0b822c9d-4755-4d0f-8395-4f31229c1dbe.png)
![image](https://user-images.githubusercontent.com/69948118/231134111-e34c7f78-62c7-49d1-a12c-4a8003c07dd7.png)
![image](https://user-images.githubusercontent.com/69948118/231134294-3439fb7a-fce7-45e8-9097-3c313934a073.png)
![image](https://user-images.githubusercontent.com/69948118/231134593-87399a17-8bec-477e-a688-9f7e88899bb5.png)
![image](https://user-images.githubusercontent.com/69948118/231134682-2f7101af-0130-4bc1-95d9-1fb9f5d486df.png)

## Terraform
![image](https://user-images.githubusercontent.com/69948118/231138767-291eb8c3-d36b-4e42-91cb-b8f3bfe9c94e.png)
![image](https://user-images.githubusercontent.com/69948118/231138911-da03608d-30a0-4868-94ef-90cc3463e542.png)
![image](https://user-images.githubusercontent.com/69948118/231139303-a06c65a2-8498-4373-92e5-f49774177289.png)
![image](https://user-images.githubusercontent.com/69948118/231139407-b4724917-3f0b-4a56-8f99-7bbe726a596a.png)
![image](https://user-images.githubusercontent.com/69948118/231139485-f5ca4045-1eeb-42ff-b27f-1ea0c0037c03.png)
## Introduction to Infrastructure as Code
![image](https://user-images.githubusercontent.com/69948118/231140584-7154d40a-dca7-448e-b9e9-f34225e355a0.png)
![image](https://user-images.githubusercontent.com/69948118/231141204-0eea380b-a710-4b81-bd9d-9c69888f23f8.png)
![image](https://user-images.githubusercontent.com/69948118/231141339-a78e17a5-b35f-4f85-a303-0a3601e81119.png)
![image](https://user-images.githubusercontent.com/69948118/231141626-15ace00c-fa27-4988-94d3-f85ef3cb490f.png)
![image](https://user-images.githubusercontent.com/69948118/231141825-c626f93f-8cf1-4e3f-8c8c-32892c55a5ed.png)
![image](https://user-images.githubusercontent.com/69948118/231142014-146e60b7-cf6c-4c51-adee-a3c5131a1158.png)
![image](https://user-images.githubusercontent.com/69948118/231142196-d9a2e4f7-fe17-4707-843e-5b5095bf1937.png)
![image](https://user-images.githubusercontent.com/69948118/231142419-b112b451-449f-4b8e-96f5-0d89819832a6.png)
### Why terraform
![image](https://user-images.githubusercontent.com/69948118/231142669-ad881d33-1178-4085-bf57-ea20aca43034.png)
![image](https://user-images.githubusercontent.com/69948118/231142839-8493ac79-43b0-4484-ba5d-d33ea030aa4b.png)
![image](https://user-images.githubusercontent.com/69948118/231142946-3beeb3dc-2397-4e9f-87bc-b90d6092d2e0.png)
![image](https://user-images.githubusercontent.com/69948118/231143234-49230559-b31f-4ea7-b7d3-fde66fce9c67.png)
![image](https://user-images.githubusercontent.com/69948118/231143557-68dfb912-a26b-493a-9e3e-b45aabb5d0ae.png)
![image](https://user-images.githubusercontent.com/69948118/231143653-a8b69033-c226-4f5f-b702-d24f0fe6c2eb.png)

## Getting Started with terraform
![image](https://user-images.githubusercontent.com/69948118/231145160-a58817ca-0c7e-4268-bb71-df62c128bc73.png)
![image](https://user-images.githubusercontent.com/69948118/231321408-e946f878-5a3d-4888-a506-87534f4c7d08.png)
![image](https://user-images.githubusercontent.com/69948118/231321512-bdf01685-04c9-48c2-8afa-e3069fc0f0e4.png)
![image](https://user-images.githubusercontent.com/69948118/231321701-8d1abd5a-d495-4794-9092-71a0c20c2afc.png)
![image](https://user-images.githubusercontent.com/69948118/231321845-6217e424-8763-4474-8110-49d3aa7edeec.png)
![image](https://user-images.githubusercontent.com/69948118/231322129-8f0d9100-86e7-46a0-852a-c9cde82a22ed.png)
![image](https://user-images.githubusercontent.com/69948118/231322350-a4c7f111-7ac9-4e37-abe6-6e3f0285d909.png)
![image](https://user-images.githubusercontent.com/69948118/231322371-3986ed6b-2bb9-4220-9fe4-1d87bd33c3f7.png)
![image](https://user-images.githubusercontent.com/69948118/231322465-520df56e-8136-4e54-bdbb-468683278e56.png)
![image](https://user-images.githubusercontent.com/69948118/231322574-086ae890-8d1e-4f7c-ab72-d459ab9e344e.png)
![image](https://user-images.githubusercontent.com/69948118/231322694-4a898e95-36b3-4f9d-b3b8-81b4dd5c1f26.png)
![image](https://user-images.githubusercontent.com/69948118/231322778-6215af59-675c-4d2a-ab4e-86c7f6df63c4.png)
![image](https://user-images.githubusercontent.com/69948118/231322844-6a7df97e-33e1-4fd5-838c-4d12f82e28c1.png)
![image](https://user-images.githubusercontent.com/69948118/231323026-52f2525a-b5ef-4e93-88a1-499cc8a64ee5.png)
![image](https://user-images.githubusercontent.com/69948118/231323308-535f3111-a5dd-403b-803f-38fe72354c34.png)
![image](https://user-images.githubusercontent.com/69948118/231323495-a4c07a75-88de-4fc7-9632-de81c1c71dc7.png)
![image](https://user-images.githubusercontent.com/69948118/231323761-25eea889-3fa9-40e4-98b9-206e6a1bd459.png)
![image](https://user-images.githubusercontent.com/69948118/231323803-8e06fb3b-b3ef-4d33-9e72-0304796f9fe0.png)

## Terraform Providers
![image](https://user-images.githubusercontent.com/69948118/231325579-2152ea86-2ace-4414-886e-dcfd90c906b7.png)
- https://registry.terraform.io/providers/hashicorp/aws/latest
![image](https://user-images.githubusercontent.com/69948118/231325793-95727d19-e71e-4a11-8c1a-ee016115a1d4.png)
![image](https://user-images.githubusercontent.com/69948118/231325904-68ec6657-7625-4ab2-937f-b948bba69d48.png)
![image](https://user-images.githubusercontent.com/69948118/231326002-a62b0fec-f367-4eca-ba35-62cdd2e690df.png)
![image](https://user-images.githubusercontent.com/69948118/231326029-e131a6d1-b47d-451f-95e9-29d5b8804ab7.png)
### Configuration directory
![image](https://user-images.githubusercontent.com/69948118/231329441-5f899f76-5f6f-483a-bef7-2f1c05ddfc4c.png)
![image](https://user-images.githubusercontent.com/69948118/231329521-6a11a6eb-4288-418d-8508-b87cf9234701.png)
### Multiple  providers
![image](https://user-images.githubusercontent.com/69948118/231329771-43bbc7b0-d41b-4b0d-a19f-40f552ebb78c.png)
### Define Input Variables
![image](https://user-images.githubusercontent.com/69948118/231333228-f74cbac5-480d-4356-9b0c-38df768ea085.png)
![image](https://user-images.githubusercontent.com/69948118/231333355-950d4520-53d9-4856-b718-b6de5929725b.png)
![image](https://user-images.githubusercontent.com/69948118/231333491-b38099d8-70bf-4da3-82df-b739fd81243b.png)
![image](https://user-images.githubusercontent.com/69948118/231333668-d3c61c41-a06c-4475-aad3-0fb70ce3d1fa.png)
![image](https://user-images.githubusercontent.com/69948118/231333822-d22706d4-5ece-4821-936c-e1573a3b060b.png)
![image](https://user-images.githubusercontent.com/69948118/231333944-fa62f428-5061-48df-9bf6-f2af1d6c4172.png)
![image](https://user-images.githubusercontent.com/69948118/231334097-abc6de13-02a5-4fa6-a94a-57cf9b18eb94.png)
![image](https://user-images.githubusercontent.com/69948118/231334303-17b0c3f1-3bc0-454b-81e2-dd49e99277e1.png)
![image](https://user-images.githubusercontent.com/69948118/231334374-6fb02ea3-b01a-4a29-9eb9-dd132c4f99be.png)
![image](https://user-images.githubusercontent.com/69948118/231334456-f8cef092-c0c9-401c-a007-b63f10cae013.png)
![image](https://user-images.githubusercontent.com/69948118/231334503-7bfc423a-1e2d-42fc-ac4a-5a848d3a9b85.png)
![image](https://user-images.githubusercontent.com/69948118/231334806-3c5f622c-a164-43ae-bc04-d1931a965add.png)
![image](https://user-images.githubusercontent.com/69948118/231334976-48a7d116-7b16-4d0e-8fae-cd07797f24d6.png)
### Using variables
![image](https://user-images.githubusercontent.com/69948118/231336312-a33ccf1f-ce8f-43c4-8eff-41f37c102e64.png)
![image](https://user-images.githubusercontent.com/69948118/231336341-a9161fb4-1629-4367-87cc-3c9fce1f7cbf.png)
![image](https://user-images.githubusercontent.com/69948118/231336355-73e73985-8c55-4961-85e4-5b62af8f831d.png)
![image](https://user-images.githubusercontent.com/69948118/231336405-b09e855e-8596-4a74-a271-3e7ab29e978c.png)
![image](https://user-images.githubusercontent.com/69948118/231336493-505c9155-fa1d-4269-a5cf-8c5d22e7d545.png)
![image](https://user-images.githubusercontent.com/69948118/231336583-b464e233-94f1-4033-bbc2-f93f0b85f02f.png)
![image](https://user-images.githubusercontent.com/69948118/231336931-4d795f47-22f9-4f25-9e75-87808be83b89.png)
### Resource Attribute Reference
![image](https://user-images.githubusercontent.com/69948118/231338133-7af3d115-2ecd-4aa9-b211-51c0ee771b89.png)
![image](https://user-images.githubusercontent.com/69948118/231338195-32864b45-b1d7-4d87-8168-68b5e803b859.png)
## Resource dependency
![image](https://user-images.githubusercontent.com/69948118/231348996-bcad3496-cc76-439e-b931-d84692fc37d2.png)
![image](https://user-images.githubusercontent.com/69948118/231349128-47e3e4fc-b1a7-4c1c-94b2-924cc8ffaf0d.png)
### Output variables
![image](https://user-images.githubusercontent.com/69948118/231351647-28055ed9-bb33-46f6-9c81-fa9097c533bd.png)
![image](https://user-images.githubusercontent.com/69948118/231351689-c7826096-1f82-4b50-b2c7-20bedc1f0fa4.png)
![image](https://user-images.githubusercontent.com/69948118/231351779-9deb8631-01a6-4594-8a85-dee46896ea1a.png)
![image](https://user-images.githubusercontent.com/69948118/231351861-0cd50861-267a-42ac-b8e4-89c7b5d86dbd.png)

## Inroduction to Terraform State
![image](https://user-images.githubusercontent.com/69948118/231419474-4429c160-45ad-4b66-aae3-f3d754cf238b.png)
![image](https://user-images.githubusercontent.com/69948118/231419573-31ed25c0-9f14-4c51-8f6f-c7061574d8f7.png)
![image](https://user-images.githubusercontent.com/69948118/231419859-5999e6df-4d22-43a4-a9af-b22bd86ee80b.png)
![image](https://user-images.githubusercontent.com/69948118/231420102-e8324861-d68a-4af2-b014-cf6f4b1a70d7.png)
![image](https://user-images.githubusercontent.com/69948118/231420215-bb69452c-bc80-49aa-9019-417b01003633.png)
![image](https://user-images.githubusercontent.com/69948118/231420729-4d49e8fd-0084-4e64-917a-4c7f0a88500d.png)
![image](https://user-images.githubusercontent.com/69948118/231421256-202a2473-fe0b-423e-abca-a49b806dd16b.png)
![image](https://user-images.githubusercontent.com/69948118/231421614-c8774c50-73c6-4c1e-8eec-e725d0b57c50.png)
![image](https://user-images.githubusercontent.com/69948118/231421895-f8bca584-1c05-4914-bd2d-68c554fdd677.png)
![image](https://user-images.githubusercontent.com/69948118/231422063-e2bef9eb-7181-4b93-a5ce-e6ed2c2a06fe.png)
![image](https://user-images.githubusercontent.com/69948118/231424233-c209868d-9e78-41b0-89fc-5082062b592a.png)
![image](https://user-images.githubusercontent.com/69948118/231424588-c3e25220-98f5-42b0-9b83-fd3d33f8448b.png)

## Terraform commands
![image](https://user-images.githubusercontent.com/69948118/231424989-4b36ff28-bb28-4dfa-8e1d-04eedb95b75f.png)
![image](https://user-images.githubusercontent.com/69948118/231425172-2035097c-242c-4d62-b999-adcb421f3d23.png)
![image](https://user-images.githubusercontent.com/69948118/231425341-d22a8410-5f57-4d79-b4ab-84f0d505b238.png)
![image](https://user-images.githubusercontent.com/69948118/231425530-ff099a63-79bf-4455-909b-07be956dbc50.png)
![image](https://user-images.githubusercontent.com/69948118/231425727-bef61806-0de7-4544-a506-f48672daf19d.png)
![image](https://user-images.githubusercontent.com/69948118/231426011-32152eee-ce15-4082-b0fb-bbb1be9bd063.png)
![image](https://user-images.githubusercontent.com/69948118/231426049-2f655c9f-b6cd-495d-b0c8-1bca81b17729.png)
![image](https://user-images.githubusercontent.com/69948118/231429895-20141ed1-2b12-4a20-a0c7-8334aa1b80fb.png)
![image](https://user-images.githubusercontent.com/69948118/231430529-8d6894a1-cbb9-4a1a-802e-b40b58831008.png)
![image](https://user-images.githubusercontent.com/69948118/231430779-474776e9-02f7-4dc9-b0c5-a49aea51ce07.png)
![image](https://user-images.githubusercontent.com/69948118/231430876-e0d92819-9f27-43a0-960e-ae11fd447cbe.png)
![image](https://user-images.githubusercontent.com/69948118/231431259-d9767cca-6fce-4153-b02b-4e41d6bac67e.png)
![image](https://user-images.githubusercontent.com/69948118/231431529-af72803e-1c93-4cc7-9f8b-08335c497e12.png)
![image](https://user-images.githubusercontent.com/69948118/231431624-f767ed67-67b3-4fc4-878e-f228e385938c.png)
![image](https://user-images.githubusercontent.com/69948118/231434731-58feb2a6-d7fc-4386-abce-8dfac84f403a.png)
![image](https://user-images.githubusercontent.com/69948118/231435084-331a97f2-db91-49d5-8529-6973073d2345.png)
![image](https://user-images.githubusercontent.com/69948118/231435280-afbcaecd-abc0-4e77-8ab5-32ced1df02e4.png)
![image](https://user-images.githubusercontent.com/69948118/231435366-cfe8ea2c-7bc9-41df-8eff-42f7e16e4318.png)
![image](https://user-images.githubusercontent.com/69948118/231437047-35cc1a9d-4ddf-4f21-ad7a-571c19066d3a.png)
![image](https://user-images.githubusercontent.com/69948118/231437179-c272682b-32fc-488d-a600-52dc708d4be8.png)
![image](https://user-images.githubusercontent.com/69948118/231437296-9b876d6e-3097-4431-bdc0-f790276e7a7a.png)
![image](https://user-images.githubusercontent.com/69948118/231437581-21f747e7-f145-4992-bf51-f99a565333ac.png)
![image](https://user-images.githubusercontent.com/69948118/231437639-0b8571ef-9699-4026-91d8-a2a012e78afe.png)
![image](https://user-images.githubusercontent.com/69948118/231437869-ce36066d-c8ec-475c-be2a-211d13964e64.png)
![image](https://user-images.githubusercontent.com/69948118/231437899-45a24bbb-ee52-48f7-80c9-aefeaa3dafba.png)
![image](https://user-images.githubusercontent.com/69948118/231438439-0e7a4d87-fb0c-46da-963a-4b6da47892b7.png)
![image](https://user-images.githubusercontent.com/69948118/231439299-04f98eeb-77b8-40c0-8db8-bb4ca88c6b12.png)
![image](https://user-images.githubusercontent.com/69948118/231439383-cb5fb4c4-cb75-411f-aecc-4a058ea4f591.png)
![image](https://user-images.githubusercontent.com/69948118/231439586-31a17798-231a-4e52-8187-225c04fa186c.png)
![image](https://user-images.githubusercontent.com/69948118/231439644-ca5f7555-8748-40d2-b327-1b03d6725461.png)
![image](https://user-images.githubusercontent.com/69948118/231439729-4b617726-42cb-44fb-9da4-e02ceb3b7a74.png)
![image](https://user-images.githubusercontent.com/69948118/231441390-418da6f8-a72c-4c7d-99ff-572572dd7c77.png)
![image](https://user-images.githubusercontent.com/69948118/231442166-dac1d2bb-9f94-4293-85a6-f96f79d5672f.png)

## Lab Setup
![image](https://user-images.githubusercontent.com/69948118/231444207-3cbd2f18-f5dd-4da2-a00e-a5888b2f33ae.png)
![image](https://user-images.githubusercontent.com/69948118/231444466-a9f3bba7-780a-4833-a1e9-22599ffa751c.png)
![image](https://user-images.githubusercontent.com/69948118/231444651-3ef4d9a4-a223-452e-b0c6-186138bd2aab.png)
![image](https://user-images.githubusercontent.com/69948118/231444751-d1fd6bbc-9828-472e-b013-34412a307bdd.png)
![image](https://user-images.githubusercontent.com/69948118/231444905-be590dab-5195-4a84-a31f-f141cf6cc0ad.png)
![image](https://user-images.githubusercontent.com/69948118/231445015-d1c9ee62-166c-4e55-b1a3-a6b1eaef3241.png)
![image](https://user-images.githubusercontent.com/69948118/231445186-22d403c8-f199-493c-a3df-fa657f2f40db.png)
![image](https://user-images.githubusercontent.com/69948118/231445317-bdb9d41c-dbb5-4f8a-9e13-fe865f275e17.png)













