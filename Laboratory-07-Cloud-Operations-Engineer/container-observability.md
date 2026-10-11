## Application Logging

### HTTP 404 Error Log

`172.17.0.1 - - [11/Oct/2026:11:13:58 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"`

### Explanation

Application logs help identify errors and show the requests made to the web application. They are vital for troubleshooting because they help engineers locate problems and understand what happened when an error occurred.


## Real-Time Container Metrics

- Container Name: client-website
- Memory Usage: 2.734MiB
- Memory Limit: 1.859GiB
- CPU Usage: 0.00%
- Memory Percentage: 0.14%
- Network I/O: 3.8kB / 5.25kB
- Block I/O: 0B / 12.3kB
- PIDs: 2

The `docker stats` command was used to monitor the container's resource consumption in real time. The client-website container was using 2.734MiB of memory and 0.00% CPU at the time of observation.
