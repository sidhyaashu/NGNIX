```plaintext

main
├── events
│   ├── worker_connections
│   ├── use
│   └── multi_accept
├── http
│   ├── include
│   │   └── mime.types
│   ├── default_type
│   ├── log_format
│   ├── access_log
│   ├── error_log
│   ├── sendfile
│   ├── keepalive_timeout
│   ├── server
│   │   ├── listen
│   │   ├── server_name
│   │   ├── root
│   │   ├── index
│   │   ├── location
│   │   │   ├── /
│   │   │   │   ├── proxy_pass
│   │   │   │   ├── try_files
│   │   │   │   └── ...
│   │   │   ├── /api
│   │   │   │   ├── proxy_pass
│   │   │   │   └── ...
│   │   │   └── ...
│   │   ├── ssl_certificate
│   │   ├── ssl_certificate_key
│   │   ├── location ~ \.php$
│   │   │   ├── include
│   │   │   ├── fastcgi_pass
│   │   │   └── ...
│   │   └── ...
│   ├── upstream
│   │   ├── backend_servers
│   │   │   ├── server server1:port
│   │   │   ├── server server2:port
│   │   │   ├── weight
│   │   │   └── ...
│   │   └── ...
│   ├── add_header
│   ├── charset
│   ├── client_max_body_size
│   ├── ...
└── stream
    ├── server
    │   ├── listen
    │   ├── proxy_pass
    │   ├── ssl_preread
    │   ├── ...
    ├── upstream
    │   ├── backend_servers
    │   │   ├── server server1:port
    │   │   ├── server server2:port
    │   │   └── ...
    │   └── ...
    └── ...

```