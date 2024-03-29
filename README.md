# Singleton SD - DOCKER Gitlab-CI VALIDATOR

Contains necessary files to create docker images with gitlab-ci validator.

> The **main repository** is hosted in [gitlab.com/singletonsd/docker/gitlab-ci-validator](https://gitlab.com/singletonsd/docker/gitlab-ci-validator.git) but it is automaticaly mirrored to [github.com/singletonsd](https://github.com/singletonsd/docker-gitlab-ci-validator.git), [github.com/patoperpetua](https://github.com/patoperpetua/docker-gitlab-ci-validator.git) and to [gitlab.com/patoperpetua](https://gitlab.com/patoperpetua/docker-gitlab-ci-validator.git). If you are in the Github page it may occur that is not updated to the last version.

## IMAGES

- **singletonsd/docker/gitlab-ci-validator/alpineXXX:** alpine base image. Available versions:
  - **3.7**
  - **3.8**
  - **3.9**
  - **edge**
- **singletonsd/docker/gitlab-ci-validator/debianXXX:**debian base image. Available versions:
  - **8**
  - **9**
  - **10**

## DOCUMENTATION

- [Github Code0x58 Gitlab-CI Validate](https://github.com/Code0x58/gitlab-ci-validate)

## HOW TO SETUP PROXY

Execute the following code to create the necessary folders:

```bash
mkdir -p .docker/.proxy
```

Create a file inside **.proxy** folder called **config.json. Inside it, write the following (make the changes to your actual proxy configuration):

```json
{
  "proxies": {
    "default": {
      "httpProxy": "http://****proxyIP****:***proxyPort***",
      "httpsProxy": "http://****proxyIP****:***proxyPort***",
      "ftpProxy": "http://****proxyIP****:***proxyPort***"
    }
  }
}
```

----------------------

© [Singleton SD](http://singletonsd.com), Italy, 2019.
