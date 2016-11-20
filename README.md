# pynginx-accesstail

pynginx-accesstail is a python script to parse an NGINX Access.log file.

It requires the following NGINX log_format directive:

> log_format main '$remote_addr - $http_x_forwarded_for - $http_x_realip - '
>                 '[$time_local] $scheme $http_x_forwarded_proto $http_x_forwarded_proto_or_scheme '
>                 '"$request" $status $body_bytes_sent "$http_referer" "$http_user_agent"';

## USAGE

> python tail.py [accesslogfile]

If no logfile is provided the user will be prompted for a file path
