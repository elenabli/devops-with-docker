# DevOps with Docker

My exercise solutions for [DevOps with Docker](https://devopswithdocker.com/), the University of Helsinki's course on containers, run with Eficode. I completed all three parts.

## Part 1: Docker basics

`part-1/exercise1.1` to `exercise1.15`: running and inspecting containers, comparing image sizes, writing Dockerfiles for a Java app and for a frontend and backend, and publishing an image to Docker Hub ([wasm-search-widget](https://github.com/elenabli/wasm-search-widget)). `part-1/practice` holds small examples from the course material.

## Part 2: Docker Compose

`part-2/ex2.1` to `ex2.8`: Compose files for a multi-container app, step by step: frontend and backend, a Redis cache, and an nginx reverse proxy in front of both.

## Part 3: Deployment pipeline

`part-3/express-app`: a small Express app with a GitHub Actions workflow that builds a multi-platform image (amd64 and arm64) and pushes it to Docker Hub on every push to `main`. The Compose file runs the image together with Watchtower, which pulls each new version automatically.

The workflow lives in `part-3/express-app/.github/workflows`, so it doesn't run in this repository. It ran in the app's original repository, which is where its commit history comes from.
