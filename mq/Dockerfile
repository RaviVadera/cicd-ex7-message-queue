FROM rabbitmq:3
USER rabbitmq
HEALTHCHECK --interval=2s --timeout=5s --start-period=1s --retries=15 CMD rabbitmq-diagnostics -q check_running && rabbitmq-diagnostics -q check_local_alarms