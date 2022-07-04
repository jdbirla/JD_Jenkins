# Java Techi Jenkins
src: https://www.youtube.com/watch?v=1QLMqyFFEzU&list=PLVz2XdJiJQxwS0BZUHX34ocLTJtRGSQzN&index=2

![image](https://user-images.githubusercontent.com/69948118/177058667-de8632d2-81a5-4496-b7e9-2d4ac2c3a897.png)
![image](https://user-images.githubusercontent.com/69948118/177058684-c3d6153a-fcb1-4a42-a7e3-844722c1ee65.png)
![image](https://user-images.githubusercontent.com/69948118/177058711-c5b8d637-a2f0-41af-9cf0-e493d60ccae5.png)
![image](https://user-images.githubusercontent.com/69948118/177058754-17216a47-b74a-423c-ad57-58cb94c47d34.png)
![image](https://user-images.githubusercontent.com/69948118/177058782-54663747-cc06-4f5f-bb2d-339cd5c08a12.png)
![image](https://user-images.githubusercontent.com/69948118/177058816-b163ddd2-181b-41bb-a43c-f09b1f6c3db8.png)
![image](https://user-images.githubusercontent.com/69948118/177058829-07dd8655-7982-4e74-88c6-88535b5df80b.png)

## Install Jenkins
![image](https://user-images.githubusercontent.com/69948118/177058893-9279c392-8704-4864-90fe-30481c592483.png)
![image](https://user-images.githubusercontent.com/69948118/177058921-dbea3af0-6dc4-4437-b974-441708927cbd.png)
![image](https://user-images.githubusercontent.com/69948118/177059001-e16653f1-1e46-4f73-956d-76a10b69e746.png)
![image](https://user-images.githubusercontent.com/69948118/177059172-bbb80b4b-9ede-4651-bb12-f5592296eebb.png)
![image](https://user-images.githubusercontent.com/69948118/177060064-e3e42a2b-970e-42e7-9a19-a85bd54c9b1e.png)
- Create a spring project or any java project
![image](https://user-images.githubusercontent.com/69948118/177060116-f70628f1-f037-4615-8399-a8d4a74ad059.png)
- Create new repository spring-jenkins
- ![image](https://user-images.githubusercontent.com/69948118/177060277-04534605-1543-4794-8d3a-63ba4c558b37.png)
- Create a new job
- ![image](https://user-images.githubusercontent.com/69948118/177060316-7a4a4a62-f2ad-4684-89d1-454f480acf93.png)
- ![image](https://user-images.githubusercontent.com/69948118/177060349-270afd3f-d5dc-4bad-b0a3-3f1f427fc795.png)
- ![image](https://user-images.githubusercontent.com/69948118/177060392-abb62b8c-df85-4982-b4a5-302e7dac5169.png)
- Schedule job cron expression
- ![image](https://user-images.githubusercontent.com/69948118/177060406-78b7a8e4-c5ca-41da-a8d2-98b982ce464a.png)
- ![image](https://user-images.githubusercontent.com/69948118/177060434-ee1a1b84-8020-485f-bbca-84bb7d480182.png)
- ![image](https://user-images.githubusercontent.com/69948118/177060462-bb83ea8e-3881-49c7-b465-e8fce29d1e67.png)
- ![image](https://user-images.githubusercontent.com/69948118/177060480-22a1fc3b-df34-4488-b10f-1852c1636381.png)
- When we changed in code , commit and pushed build will automaticall triggered
- ![image](https://user-images.githubusercontent.com/69948118/177060577-71a1cc6f-2fd7-4487-8f23-8d8930096257.png)
- When build fail
- ![image](https://user-images.githubusercontent.com/69948118/177060642-63220365-61eb-4d08-947d-ec076bc3db4f.png)
- ![image](https://user-images.githubusercontent.com/69948118/177060656-1ce6639a-94f7-4a0f-81e5-a04ab346f482.png)
- Email configuration
- ![image](https://user-images.githubusercontent.com/69948118/177060702-72c9f9fe-d7e6-40ad-89a1-8f1cd49b1fd8.png)
- ![image](https://user-images.githubusercontent.com/69948118/177060760-3a1adae8-3495-42e0-bc7b-7e227701ef6d.png)
### Continuous Integration Pipeline
- ![image](https://user-images.githubusercontent.com/69948118/177060991-752336df-7517-4e4e-bceb-ced0d1efb8b9.png)
- ![image](https://user-images.githubusercontent.com/69948118/177061018-dfb91c3a-3260-4bfb-8c0b-c895c39ae91a.png)
- ![image](https://user-images.githubusercontent.com/69948118/177061046-be295c04-681f-48d1-a67a-dfbf284b4a6d.png)
- ![image](https://user-images.githubusercontent.com/69948118/177061057-dc0fbbaf-fd2b-4b82-b998-14db4dd561d6.png)
- ![image](https://user-images.githubusercontent.com/69948118/177061092-b534388a-553b-4b50-b2b4-80e45ab5e9ca.png)
- ![image](https://user-images.githubusercontent.com/69948118/177061104-0977b9b8-9fa2-45ab-95b3-c6011c3ad73b.png)
- Create build pipeline
- Create new job as DEV maven goal will be ```install```
- ![image](https://user-images.githubusercontent.com/69948118/177061138-f2dd4556-b08c-457a-9d1a-6b80e3b886ad.png)
- Create new job UAT maven goal will be ``` test ```
- ![image](https://user-images.githubusercontent.com/69948118/177061239-e081492f-3aa3-4086-bc5c-6c4782a84490.png)
- Create new job PROD maven goal will  be ```install``
- ![image](https://user-images.githubusercontent.com/69948118/177061289-2903b73b-aff1-40af-9fa4-8bf44f941d7e.png)
- Create build pipeline using build pipeline plugin please install plugin before create pipeline else option won't available
- ![image](https://user-images.githubusercontent.com/69948118/177061360-901de8fb-b6ab-437b-b6ed-449bb7977618.png)
- ![image](https://user-images.githubusercontent.com/69948118/177061402-3e245edd-8c94-4d92-a751-287b32734b84.png)
- ![image](https://user-images.githubusercontent.com/69948118/177061426-c52bd948-7d04-410b-a610-c9a3d42a44e7.png)
- ![image](https://user-images.githubusercontent.com/69948118/177061435-caae9764-c51a-4755-b7c8-b7d85475196e.png)
- Configure each pipeling for after which job it has to run like DEV -> UAT -> PROD
- ![image](https://user-images.githubusercontent.com/69948118/177061510-c147a162-a4d0-4ccb-a609-22e9ead8ed81.png)
- ![image](https://user-images.githubusercontent.com/69948118/177061556-84048651-ace5-4ad9-a1b9-05c9320260f5.png)
-  Do some code change and commit
- ![image](https://user-images.githubusercontent.com/69948118/177061622-ccce8370-3612-48a1-8af2-1392f7abf8a4.png)
- ![image](https://user-images.githubusercontent.com/69948118/177061641-9eb05ea5-d755-46d4-89b3-71ff2e00107c.png)

- Building Docker Images using Jenkins step by step 
![image](https://user-images.githubusercontent.com/69948118/177067958-2b633918-f5af-42aa-a67c-06702e56491e.png)
- Create new job
- ![image](https://user-images.githubusercontent.com/69948118/177068858-b0cb5dda-96cd-4cb9-a051-3f8662199735.png)
- ![image](https://user-images.githubusercontent.com/69948118/177068890-c9e11d76-9c0b-4138-a6a0-6f7e1dc8c2a2.png)
- ![image](https://user-images.githubusercontent.com/69948118/177068956-ad832eec-377f-4394-83a6-1874666a8520.png)
- ![image](https://user-images.githubusercontent.com/69948118/177068997-d2b85a6f-68ca-41c8-b12e-d5a05a5e9d3e.png)
- In order to connect Jenkins with Docker we need to add some below plugins 
- ![image](https://user-images.githubusercontent.com/69948118/177069560-382ba100-7b96-4a48-a14e-4e86cd615467.png)
- ![image](https://user-images.githubusercontent.com/69948118/177069583-c88e1051-6bb8-4c8c-916b-28eabffac341.png)
- We need to create docler file
- ![image](https://user-images.githubusercontent.com/69948118/177069811-cbeddddc-ffb9-44a1-b443-0923a9af7bf0.png)
- Commit and push to remote repo
- ![image](https://user-images.githubusercontent.com/69948118/177069959-4e1fe515-fb37-43e9-b790-ab2fda5b9477.png)
- ![image](https://user-images.githubusercontent.com/69948118/177070122-8ec4b9bb-fc24-4159-be78-1f54291f2828.png)
- Start a build
- ![image](https://user-images.githubusercontent.com/69948118/177070152-fb009ce1-74f2-4c27-8c45-efdf985cdd35.png)
---
### Build Docker image using Jenkins pipeline and puch to Docker hub
- 
- ![image](https://user-images.githubusercontent.com/69948118/177070643-1e649393-d950-41be-8bf0-761c420b5a69.png)
-  Create Pipeline
-  ![image](https://user-images.githubusercontent.com/69948118/177077113-63065d4c-6100-429d-beac-17630da22322.png)
- ![image](https://user-images.githubusercontent.com/69948118/177077151-05a637f8-ea35-446d-b2d4-e058e87cff06.png)
- ![image](https://user-images.githubusercontent.com/69948118/177077200-d1e54b9e-931d-45c6-948d-b0bd46b429d3.png)
- ![image](https://user-images.githubusercontent.com/69948118/177077281-27dba9a6-a4e8-4c35-9729-3290dc2945cb.png)
- ![image](https://user-images.githubusercontent.com/69948118/177077369-7cc74eac-c1d0-4237-9b9a-ebb1ee98c93f.png)
- ![image](https://user-images.githubusercontent.com/69948118/177077422-d1336a5f-0333-4904-a480-b8eb4758ea69.png)
- ![image](https://user-images.githubusercontent.com/69948118/177077765-52f73929-2d29-4705-878c-b17011f14138.png)
- Docker file 
- ![image](https://user-images.githubusercontent.com/69948118/177077940-3b83cb49-10f0-46b7-b675-a8bb45c07490.png)
- Commit the docker file
- 
![image](https://user-images.githubusercontent.com/69948118/177078376-13adc9a3-08ba-425d-a0bd-2ad5aff058be.png)
- We can create user and password environment variable 
- ![image](https://user-images.githubusercontent.com/69948118/177078805-e890556a-69b4-42cc-b231-f026676ff195.png)
- ![image](https://user-images.githubusercontent.com/69948118/177080515-92e09569-833b-428e-8e66-dd9b20edb919.png)
- ![image](https://user-images.githubusercontent.com/69948118/177080557-e880a83d-0d8a-4b6f-ae6e-be3f1c80a9a8.png)
- ![image](https://user-images.githubusercontent.com/69948118/177080699-b4a60a44-af8f-40ca-9d69-3b098c9c0601.png)

- After Configuration build now
- ![image](https://user-images.githubusercontent.com/69948118/177080894-deacc378-77f5-452c-ae28-099ba5f4bd86.png)

- Another way we can commit ```Jenkinsfile``` in github
- ![image](https://user-images.githubusercontent.com/69948118/177081251-7fbd08b5-21d0-4452-81fd-24db7d58c4a8.png)
- 

---
### CI CD Pipeline Using Jenkins | Deploy Docker Image to Kubernetes using Jenkins












