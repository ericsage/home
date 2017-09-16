
Sage Code
===========
My complete development environment inside of a Docker image!

What's inside
-------------
- Based on [Alpine Linux](https://hub.docker.com/_/alpine/) for the smallest footprint possible.
- Colorscheme agnostic UI
- Golang, Python3, Nodejs
- Gcloud, AWS, Docker, and Kubernetes CLIs
- [Vim plugins](https://github.com/ericsage/code/blob/master/configfiles/.vimrc#L27-L74)
- [Alpine packages](https://github.com/ericsage/code/blob/master/packages/apk)
- [Python packages](https://github.com/ericsage/code/blob/master/packages/pip)

Sample Usage
------------
```bash
docker run -it --name code \
-v ~/Documents/Secrets/aws:/root/.aws \
-v ~/Documents/Secrets/key:/root/.key \
-v ~/Documents/Code:/root/Code/src \
-v /var/run/docker.sock:/var/run/docker.sock \
ericsage/code
```