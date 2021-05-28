# XNAT build

```console
# Download pre-requisite files
$ make

# Build all images
$ packer build xnat-web.pkr.hcl

# Build an individual image
$ packer build -only docker.xnat17 xnat-web.pkr.hcl

# Build all docker images
$ packer build -only docker.* xnat-web.pkr.hcl

# push images to local repository
$docker push localhost:32000/xnat-web:1.8.1-dev
```

Reference:
* https://bitbucket.org/xnatdev/container-service/downloads/
