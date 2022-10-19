### Deploying Flask Application on Cloud Run using CI-CD Pipeline 

1. Enable Cloud Source Repository API & create a new repository by giving meaningful repo name and choosing Project ID on which you are going to Work

2. Next step, Add code to your repository by following below commands on CloudShell.

    # a) gcloud init
    
    # b) gcloud source repos clone REPO_NAME --project=PROJECT_ID
    
    # c) cd REPO_NAME
    
    # d) git add -A
    
    # e) git commit -m "SOME_MESSAGE"
    
    # f) git push -u origin master

3. Enable Artifact Registry API and create a repository of format Docker which will stores your docker images.

### FOLDER STRUCTURE OF REPOSITORY: "region-name-docker.pkg.dev > project id > name of the repository"

4. Enable Cloud Run API & Cloud Build API

5. Go to Cloud Build --> Click Settings first & then First enable Cloud Run, this will create a service account which will have Cloud Run Admin role which will help cloud build to create and deploy an application to Cloud Run.

6. Create a trigger and click on RUN to start the build process.
