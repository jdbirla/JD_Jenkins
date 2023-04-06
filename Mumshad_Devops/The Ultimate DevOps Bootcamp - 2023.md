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




