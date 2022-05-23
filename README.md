# JD Jenkins Leanrnings

1. simplilearn1 : https://www.youtube.com/watch?v=FX322RVNGj4
2. edureka : https://www.youtube.com/watch?v=p7-U1_E_j3w

## simplilearn1

## Overview:

![Browser](Images/Screenshot_14.png)

![Browser](Images/Screenshot_15.png)

---

## DevOps

![Browser](Images/Screenshot_16.png)

![Browser](Images/Screenshot_17.png)

![Browser](Images/Screenshot_18.png)

![Browser](Images/Screenshot_19.png)

![Browser](Images/Screenshot_20.png)

![Browser](Images/Screenshot_21.png)

![Browser](Images/Screenshot_22.png)

![Browser](Images/Screenshot_23.png)

![Browser](Images/Screenshot_24.png)

![Browser](Images/Screenshot_25.png)
---
## DevOps Tools
![Browser](Images/Screenshot_26.png)

---
## DevOps Process

![Browser](Images/Screenshot_27.png)

![Browser](Images/Screenshot_28.png)

![Browser](Images/Screenshot_29.png)

---
## DevOps Advantages

![Browser](Images/Screenshot_30.png)

![Browser](Images/Screenshot_31.png)


---
## Jenkins Installation

![Browser](Images/Screenshot_32.png)

![Browser](Images/Screenshot_33.png)

![Browser](Images/Screenshot_34.png)

![Browser](Images/Screenshot_35.png)


## Before Jenkins

![Browser](Images/Screenshot_5.png)

## What is Jenkins?

![Browser](Images/Screenshot_6.png)

## What is Continuous Integration?

![Browser](Images/Screenshot_7.png)


## Continuous Integration Tools

![Browser](Images/Screenshot_8.png)


## Features of Jenkins

![Browser](Images/Screenshot_9.png)

## Jenkins Pipeline

![Browser](Images/Screenshot_10.png)

## Jenkins Architecture

![Browser](Images/Screenshot_11.png)

## Master-Slave Architecture

![Browser](Images/Screenshot_12.png)

## Jenkins Case Study

## Key Takeaways

![Browser](Images/Screenshot_13.png)

---
## Jenkins Practice

![Browser](Images/Screenshot_36.png)

![Browser](Images/Screenshot_37.png)

![Browser](Images/Screenshot_38.png)

![Browser](Images/Screenshot_39.png)

![Browser](Images/Screenshot_40.png)

![Browser](Images/Screenshot_41.png)

![Browser](Images/Screenshot_42.png)

![Browser](Images/Screenshot_43.png)

![Browser](Images/Screenshot_44.png)

![Browser](Images/Screenshot_45.png)

![Browser](Images/Screenshot_46.png)

![Browser](Images/Screenshot_47.png)

![Browser](Images/Screenshot_48.png)

![Browser](Images/Screenshot_49.png)

![Browser](Images/Screenshot_50.png)

![Browser](Images/Screenshot_51.png)

![Browser](Images/Screenshot_52.png)

![Browser](Images/Screenshot_53.png)

![Browser](Images/Screenshot_54.png)

![Browser](Images/Screenshot_55.png)

![Browser](Images/Screenshot_56.png)

![Browser](Images/Screenshot_57.png)
---

## Distributed Build

![Browser](Images/Screenshot_58.png)

![Browser](Images/Screenshot_59.png)

![Browser](Images/Screenshot_60.png)

![Browser](Images/Screenshot_61.png)

---
## Jenkins Pipeline

![Browser](Images/Screenshot_62.png)

![Browser](Images/Screenshot_63.png)

![Browser](Images/Screenshot_64.png)

![Browser](Images/Screenshot_65.png)

![Browser](Images/Screenshot_66.png)


### pipeline basic syntax
```
pipeline {
    agent any
	stages {
        stage('Git-Checkout') {
            steps {
                echo 'Checking out from git'
            }
        }
		
	    stage('Build') {
            steps {
                echo 'Building the checkout project'
            }
        }
		
	    stage('Unit-Test') {
            steps {
                echo 'Running the unit test'
            }
        }
		
        stage('Quality-Gate') {
            steps {
                echo 'Verfying the quality gates'
            }
        }
    }
	post {
	    always{
		   echo 'This will always run'
		} 
		success{
		   echo 'This will run only if sucessful'
		} 
		failure{
		   echo 'This will run only if failed'
		} 
		unstable{
		   echo 'This will run only if the run was marked as unstable'
		} 
		changed{
		   echo 'This will only run if state  of the pipeline has been changed'
		   echo 'For example the pipeline was previouly failing but now sucessful'
		} 
	}
}

```

### pipeline basic syntax with github
```
pipeline {
    agent any
	stages {
        stage('Git-Checkout') {
            steps {
                echo 'Checking out from git';
                git 'https://github.com/jdbirla/Pipeline_Script.git'
            }
        }
		
	    stage('Build') {
            steps {
                echo 'Building the checkout project';
                bat 'Build.bat'
            }
        }
		
	    stage('Unit-Test') {
            steps {
                echo 'Running the unit test';
                bat 'Unit.bat'
            }
        }
		
        stage('Quality-Gate') {
            steps {
                echo 'Verfying the quality gates';
                bat 'Quality.bat'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying to stage env for more tests';
                bat 'Deploy.bat'
            }
        }
    }
	post {
	    always{
		   echo 'This will always run'
		} 
		success{
		   echo 'This will run only if sucessful'
		} 
		failure{
		   echo 'This will run only if failed'
		} 
		unstable{
		   echo 'This will run only if the run was marked as unstable'
		} 
		changed{
		   echo 'This will only run if state  of the pipeline has been changed'
		   echo 'For example the pipeline was previouly failing but now sucessful'
		} 
	}
}

```

![Browser](Images/Screenshot_67.png)

![Browser](Images/Screenshot_68.png)

![Browser](Images/Screenshot_69.png)

---





