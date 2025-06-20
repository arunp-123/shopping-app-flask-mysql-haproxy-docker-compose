FROM haproxy:latest

# Copy HAProxy configuration file
COPY haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg

# Copy pre-created certs folder (must exist in build context)
COPY certs /usr/local/etc/haproxy/certs

