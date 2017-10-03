# Drupal https example.

## How to use this repo.

Create network first.

```
$ docker network create -d bridge nginx-proxy
```

Then

```
$ docker-compose up
```

## Debug

Checkout the docker-gen generated "default.conf" file

~~~
$ docker exec -it nginx-gen cat /etc/nginx/conf.d/default.conf
~~~


## References

- docker-composer.yml https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion-examples/raw/c3bc75b10021d2cc268f5ed39db2211482e57813/docker-compose/v2/simple-site/docker-compose.yml
- nginx.tmpl https://github.com/jwilder/nginx-proxy/blob/f05f7a0ff965d7a5fa38b4dd567f4913ce874fe8/nginx.tmpl
- nginx-compose-v2.tmpl https://raw.githubusercontent.com/JrCs/docker-letsencrypt-nginx-proxy-companion-examples/c3bc75b10021d2cc268f5ed39db2211482e57813/volumes/proxy/templates/nginx-compose-v2.tmpl
- https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion-examples
- https://github.com/jwilder/nginx-proxy/issues/304
