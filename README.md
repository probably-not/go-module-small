# go-module-small

A template for a small and simple go module.

## What Does This Contain?
- My standard [`.gitignore`](.gitignore) file. This is the gitignore I use, mostly generated from (gitignore.io)[https://gitignore.io], with some added miscellaneous files that I use locally.
- My standard [`Dockerfile`](Dockerfile) file. This is my super basic multi-stage Dockerfile, that uses the latest Go as the build-env and Google's Distroless as the final environment.
- My standard [`Makefile`](Makefile). I like to use a Makefile so that I don't have to always remember how to build, tag, and push new docker images to my registry. The Dockerfile doesn't actually contain anything other than build and push of docker images, and a build local binary step. Linting, testing, formatting is all taken care of outside of this.
- A [`main.go`](main.go) file with no logic.