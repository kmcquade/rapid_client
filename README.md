# rapid_client

I found this in the `/var/runtime` directory of AWS's [aws-sam-cli-emulation-image-python3.8](https://hub.docker.com/r/amazon/aws-sam-cli-emulation-image-python3.8) Docker image. I was frustrated because it seems to be very difficult to build your own Python Docker image to be used with AWS SAM. It was giving me some error about missing the `AWS_LAMBDA_RUNTIME_API` environment variable, so I dove into the rabbit hole and found that their image relies on this content.

They didn't open source the code for that Docker Image on GitHub, but the code is available via their public docker image, so I thought I'd stash it here.

I've kept everything in its raw form. The only changes to this directory are:
* Added `.gitignore`, which excludes `*.dist-info` files, `.vscode/`, `.idea/` since those are pretty useless and not relevant.
* Added README

I've even kept the content of the dependencies, even though that makes it look cluttered. This way you don't have to install anything, you can view it in its original form.


