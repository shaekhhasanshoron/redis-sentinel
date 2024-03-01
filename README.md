# Redis-Sentinel

## Redis v3.0.7

### Installation

1. Update the storageClass for in [redis-sts](https://github.com/shaekhhasanshoron/redis-sentinel/blob/master/redis-3.0.7/5.redis-sts.yaml) and [redis-sentinel-sts](https://github.com/shaekhhasanshoron/redis-sentinel/blob/master/redis-3.0.7/8.redis-sentinel-sts.yaml)
2. Update storage, cpu, memory if required.
3. update/remove toleration from [redis-sts](https://github.com/shaekhhasanshoron/redis-sentinel/blob/master/redis-3.0.7/5.redis-sts.yaml) and [redis-sentinel-sts](https://github.com/shaekhhasanshoron/redis-sentinel/blob/master/redis-3.0.7/8.redis-sentinel-sts.yaml)
4. update replicas, if replicas are not '3' then update nodes in [redis-config](https://github.com/shaekhhasanshoron/redis-sentinel/blob/master/redis-3.0.7/2.redis-config.yaml) configmap.

Apply all the files under redis-3.0.7 folder

```
kubectl apply -f redis-3.0.7/
```