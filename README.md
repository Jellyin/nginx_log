# nginx log format
    log_format  main '{'
                    '"remote_addr": "$remote_addr",'
                    '"time_local": "$time_local",'
                    '"time_iso8601": "$time_iso8601",'
                    '"request_method": "$request_method",'
                    '"request_uri": "$request_uri",'
                    '"request_body": "$request_body",'
                    '"request_length": $request_length,'
                    '"server_protocol": "$server_protocol",'
                    '"server_name": "$server_name",'
                    '"host_domain": "$host",'
                    '"msec": $msec,'
                    '"status": $status,'
                    '"body_bytes_sent": $body_bytes_sent,'
                    '"http_referer": "$http_referer",'
                    '"http_user_agent": "$http_user_agent",'
                    '"request_time": $request_time,'
                    '"upstream_addr": "$upstream_addr",'
                    '"upstream_response_time": "$upstream_response_time",'
                    '"scheme": "$scheme",'
                    '"http_cookie": "$http_cookie",'
                    '"request_completion": "$request_completion",'
                    '"pipe": "$pipe"'
                  '}';
                  
# docker image:
https://hub.docker.com/r/jaylenyin/nginx/

docker run -d -p 80:80 jaylenyin/nginx
