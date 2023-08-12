# celery 启动
1. 启动 worker
```shell
celery -A celery_tasks worker -l info
```
2. 手动执行消息生产者,即可
```shell
python3 prodce_task
```

# 定时任务
1. 启动worker
2. 执行定时任务 beat
```shell
celery -A celery_tasks beat -l info 
```

# flower启动
1. 在启动了 worker，和 beat 后，再启动 flower 监控平台
