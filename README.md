# Gitops-CICD-Pipeline
GitOps with Argo CD &amp; Advanced Jenkins 
![image](https://github.com/rajeebswain/Gitops-CICD-Pipeline/assets/105234711/5cd141f2-264d-4b52-8ef7-51e4f7de925a)

### Description:
Here, the code flow is like this, when the DevOps team pushes the code, the webhook triggers a CI, that builds the source code and the final artefacts, which will be pushed to the image registry or the artefact store. Artefact means the executable files in the deployment.

Once the artefact is pushed, in the same pipeline we can call one more pipeline that will basically update your latest configuration changes like IAC code, Kubernetes manifest file with the latest image tag for that particular release.
Once configurations are updated in the configuration repository, we can raise one more PR to the configuration repo, to merge the changes to the main line. Once the changes are merged into the mainline we can deploy them into the target environment. 

### Code Flow in separate Repository:
![image](https://github.com/rajeebswain/Gitops-CICD-Pipeline/assets/105234711/84d79af1-2737-4c60-923e-e179ac918720)


### Prerequisite:
    - Kubernetes cluster
    - Jenkins Server
    - Git Repo
    - Argo CD


