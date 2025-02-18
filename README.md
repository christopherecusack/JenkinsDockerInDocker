# Jenkins Docker in Docker
Set up a Jenkins instance Docker in Docker.

Do you suffer from your Jenkins container being able to build and push images to a Docker repository?

I struggled piecing together the solution for this for awhile and I hope for those with the same issues, this finds you well. I did not want to bare metal Jenkins or run any node off a central controller. Just get the Jenkins container to build and push an image.

My initial install of the Jenkins container used a compose file with the standard image and I simply changed the compose file to the custom image defined within the Dockerfile. I rebuilt my current deployment and all worked well.

Compose to bring it up or modify a current container with missing the Docker cli. The compose file is using standard ports. Modify to your needs.

```
docker compose up -d
```

Cheers,
Chris
