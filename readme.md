Action works as a CI tool.
Any change of commit will trigger the workflow in the Action folder .github/workflows
it first request resources from GitHub and queue for the resource.
Once the resource is ready, it will start to run.
It create a working space with project code downloaded.
Once the workspace is ready, it will follow the steps defined in the workflow file:

# 1. Checkout the code
# 2. Setup Java 
# 3. Compile the code
# 3-1. Package code
# 4. Run tests
# 5. Build Docker image
# 6. Log in to JFrog Artifactory Docker registry
# 7. Push Docker image to Artifactory
