## Host Database
Update the host database of the machine to translate certain hostname into IP Address. In this case, translate the `www.lastpass.oom` hostname to `127.0.0.1` IP Address.

### Path
Linux: /etc/hosts \
Windows: C:\Windows\System32\Drivers\etc\hosts

## Docker
```sh
docker run --rm -p 80:80 -v $(pwd)/nginx.conf:/etc/nginx/conf.d/default.conf -v $(pwd)/welcome.html:/opt/lastpass/www/index.html nginx
```

## URL
[http://lastpass.oom](http://lastpass.oom)

## Google Chrome Security
Google chrome has a list of identified website that when visited, it enforced the address to use HTTPS protocol. \
Configuration page: [chrome://net-internals/#hsts](chrome://net-internals/#hsts)