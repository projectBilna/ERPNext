web: bench serve
redis_async_broker: redis-server config/redis_async_broker.conf
socketio: /usr/bin/nodejs apps/frappe/socketio.js
workerbeat: sh -c 'cd sites && exec ../env/bin/python -m frappe.celery_app beat -s scheduler.schedule'
worker: sh -c 'cd sites && exec ../env/bin/python -m frappe.celery_app worker'
redis_cache: redis-server config/redis_cache.conf