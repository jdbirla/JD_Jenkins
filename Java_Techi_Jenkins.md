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
- 














