# Config.toml

```toml
concurrent = 4
check_interval = 0

[session_server]
  session_timeout = 1800

[[runners]]
  name = "cicd-0"
  url = "https://gitlab.com/"
  token = ""
  executor = "docker"
  [runners.custom_build_dir]
  [runners.docker]
    tls_verify = false
    image = "debian:stretch"
    privileged = true
    disable_entrypoint_overwrite = false
    oom_kill_disable = false
    disable_cache = false
    volumes = ["/cache"]
    shm_size = 0
  [runners.cache]
    [runners.cache.s3]
    [runners.cache.gcs]
```


# update_runner.sh

```sh
docker pull gitlab/gitlab-runner:latest
docker stop gitlab-runner && docker rm gitlab-runner
docker run -d --name gitlab-runner --restart always \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -v `pwd`/runner:/etc/gitlab-runner \
  gitlab/gitlab-runner:latest
```