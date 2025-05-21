# Advanced Demo - CodePipeline
[AWS CodePipeline](https://docs.aws.amazon.com/codepipeline/latest/userguide/welcome.html) advance demo. 

In this demo series you're going to be implementing a full code pipeline incorportating commit, build and deploy steps.

The advanced demo consists of 5 stages:

* STAGE 1 : Configure Security & Create a Github Repo
* STAGE 2 : Configure CodeBuild to clone the repo, create a container image and store on ECR
* STAGE 3 : Configure a CodePipeline with commit and build steps to automate build on commit.
* STAGE 4 : Create an ECS Cluster, TG's , ALB and configure the code pipeline for deployment to ECS Fargate
* STAGE 5 : CLEANUP

![image](https://github.com/user-attachments/assets/9d30f1a4-784e-437e-ae6d-eb9f48f93933)


# Running Locally

The application is just an HTML file with some cat images. You can open the [index.html](./index.html) file in a browser.

To test locally what [AWS CodeBuild](https://docs.aws.amazon.com/codebuild/latest/userguide/welcome.html) builds, run the Dockerfile with

```
docker build -t containercats . && docker run -p 8080:80 containercats
```

and then go to `localhost:8080`

# Video Guides

- [Stage0](https://www.youtube.com/watch?v=MDMH_XXDbrI&t=0s) - INTRO
- [Stage1](https://www.youtube.com/watch?v=MDMH_XXDbrI&t=133s)
- [Stage2](https://www.youtube.com/watch?v=MDMH_XXDbrI&t=871s)
- [Stage3](https://www.youtube.com/watch?v=MDMH_XXDbrI&t=2556s)
- [Stage4](https://www.youtube.com/watch?v=MDMH_XXDbrI&t=3478s)
- [Stage5](https://www.youtube.com/watch?v=MDMH_XXDbrI&t=4594s)

# Acantril course
See https://github.com/acantril/learn-cantrill-io-labs/blob/master/aws-codepipeline-catpipeline/02_LABINSTRUCTIONS/STAGE1-CODECOMMIT.md