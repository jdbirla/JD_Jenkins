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

