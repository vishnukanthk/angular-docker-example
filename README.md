
Buildkit: The error message indicates that Buildkit is being used as the build frontend, and it failed to read the Dockerfile. Buildkit is an alternative builder for Docker. You might consider disabling Buildkit temporarily to see if it resolves the issue. You can do this by setting the DOCKER_BUILDKIT environment variable to 0:
-------------------- set DOCKER_BUILDKIT=0






------------------- docker build -t angular-app .