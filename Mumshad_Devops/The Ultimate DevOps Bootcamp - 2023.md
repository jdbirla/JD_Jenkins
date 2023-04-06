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







