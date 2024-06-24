# GitLab_CICD
- https://www.youtube.com/watch?v=qP8kir2GUgo&feature=youtu.be

## What is GitLab CI/CD?
First of all what is Gitlab CI/CD and why should you even care?

GitLab platform generally is striving to become THE DevOps platform or a one-stop shop for building DevOps processes for your applications.
GitLab as a DevOps platform
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/f00a4a93-328e-43ed-9a24-0407829c1ffa)

So they have exactly this roadmap and they're working towards that, which means they're actually integrating and creating new features to basically give you everything in one platform to build complete DevOps processes and big part of those processes is a CI/CD pipeline.

## What is CI/CD in simple words
So first of all what is CI/CD in simple words.

CI/CD stands for Continuous Integration and Continuous Deployment or Continuous Delivery and what it basically means is automatically and continuously testing, building and releasing code changes to the deployment environment.
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/051231fa-1795-4f82-9c43-f42644034b42)

So that means when a developer commits a new code into the Gitlab repository, Gitlab will automatically execute a CI/CD pipeline that you have configured for your project to release those code changes to the end environment, where the end users can access them:
CI/CD

But this CI/CD concept is a topic of its own. If you want to understand it on a deeper level then you can check out my video about DevOps and CI/CD pipeline, where I explain this in more detail here: What is DevOps?

But as I said in simple terms CI/CD is to continuously release your code changes to the end environment and in this crash course we will be building a simplified version of a CI/CD pipeline using Gitlab CI/CD.

## Many CI/CD platforms
Of course there are many CI/CD tools, one of the most used ones in the industry still being Jenkins. And Gitlab CI/CD is just one of those other CI/CD platforms:
Overview of CI/CD platforms
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/6aaf09e2-3404-4fcf-b324-a04981bf1b84)


### Source Code & CI/CD on same platform
All of them have their advantages and disadvantages, but a big advantage of using Gitlab to build CI/CD pipelines for your applications is that you already have your code on Gitlab, so this is an extension of your software development processes in your team, where you can also build CI/CD pipelines on the same platform:
GitLab benefit
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/162d6210-b593-494f-ad81-4161e8444f30)

So your team already works with Gitlab, you have your code there, so this is basically an additional feature that you can extend your workflows on Gitlab with and you don't need a separate tool for that. 👍

Apart from that Gitlab makes that extension very seamless by allowing you to get started without any setup effort and also having your pipeline as part of your application code compared to Jenkins for example, where you have to set up and configure the Jenkins server, create a pipeline and then connect it to the Git project:
GitLab vs Jenkins
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/b6458c14-baf3-4768-9c64-aae6531d198c)

With Gitlab you can start without any of this configuration effort and we will see that in the demo part.

## GitLab Architecture
Now if you don't have to set up anything and configure any servers to run the pipelines how does it actually work?
And this leads us to the topic of Gitlab architecture and how it works.

### GitLab Instance
You have a Gitlab instance or also called Gitlab server that hosts your application code and your pipelines and basically the whole configuration. So it knows what needs to be done.

### GitLab Runners
And connected to that Gitlab instance you have multiple Gitlab runners, which are separate machines connected to the Gitlab server machine, which are actually the ones executing
the pipelines.

So Gitlab server knows what needs to be done and Gitlab runner actually does that:
GitLab Architecture
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/4657063a-62a4-44ae-9ca4-f34188a56606)

### Managed or SaaS
And www.gitlab.com is actually a managed Gitlab instance that offers multiple managed runners already out of the box.
So these are all maintained by Gitlab and that's why you can start running your pipelines without any setup and configuration effort using this managed setup.

### Self-Managed
And this is already enough for starting out but of course for your own organization you may want to manage the runners or the whole setup yourself.
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/3a849224-1b54-42b7-91b0-e6ba8245c9cf)

So you can create partially or completely self-managed Gitlab setup as well:
Managed vs Self-Managed

In this crash course we will use Gitlab's managed infrastructure and free features to build our release pipeline. So we will not need to configure anything ourselves. 👍

## Pipeline Configuration - .gitlab-ci.yml
Now the question is how do we create a Gitlab CI/CD pipeline? 🤔

Well, following the concept of Configuration as Code or Pipeline as Code, the whole pipeline will be written in code and hosted in the applications git repository itself in a simple YAML file.

And the file has to be called .gitlab-ci.yml, so that Gitlab can automatically detect that pipeline code and execute it without any extra configuration effort from our site:
Pipeline is scripted
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/54852a63-37c7-4299-89fc-591817c5a8d4)

So in the root of the project's repository, we're going to create this YAML file and we're going to write all the pipeline configuration inside and we can actually
do that directly in the Gitlab UI as well, so we don't have to switch back and forth from the editor to Gitlab.
GitLab Editor
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/3daa231c-c8b9-4946-8a6b-871de0ac0873)

### Jobs
The tasks in the CI/CD pipeline such as running tests, building an image, deploying to a server etc. are configured as what's called 'jobs':
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/631e9bea-396f-479e-b099-389d37197bc7)

Jobs 1
Jobs 2
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/bb52a9e8-2ce2-4236-a8fb-4f0528423c96)

So Jobs are the most fundamental building block of a .gitlab-ci.yml file. They define what to do.

Each job has a name and inside the job we have a couple of
parameters or a couple of attributes or things that we want to configure for the job.

The first attribute and the only required attribute of a job is what's called a script. And script is basically, where we list any commands that should be executed for that job:
Pipeline config basic structure
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/1e5fd85c-0191-498a-814d-fd450300cf7b)

So for example for 'run tests', we need to execute `make test* for our python demo application. This is the command that needs to be executed in order to run the test, so we're going to write that command:
Pipeline config examples
![image](https://github.com/jdbirla/JD_Jenkins/assets/69948118/8599cd6b-a090-40a0-aa0f-b4babd318164)

However, in order for this to run successfully we need to do a couple of things.
