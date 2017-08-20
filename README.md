# Test app for Pluralsight course

This is a quick and dirty test node.js app cobbled together for the purposes of demonstrating a basic CI/CD workflow 
with Docker Hub for a Pluralsight video training course.

## Build docker images

CircleCI should post given request to trigger the build in Docker Hub

    curl -H "Content-Type: application/json" --data '{"build": true}' -X POST https://registry.hub.docker.com/u/pkk82/courses_pluralsight_docker-ci-workflows-2015/trigger/{!!! token}/