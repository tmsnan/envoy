FROM jaegertracing/all-in-one@sha256:f4797b092d6575b0e4bb0e3c1797560c179c4df9f069f9643d1f5ab6bcbd53d0
HEALTHCHECK \
    --interval=1s \
    --timeout=1s \
    --start-period=1s \
    --retries=60 \
    CMD wget -q --header='Content-Type:application/json' -O - http://localhost:14269/health | grep "Server available"
