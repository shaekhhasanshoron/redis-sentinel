# Redis-Sentinel

## Redis v3.0.7

### Installation

1. Update the storageClass for in [redis-sts]() and [redis-sentinel-sts]()
2. Update storage, cpu, memory if required.
3. update/remove toleration from [redis-sts]() and [redis-sentinel-sts]()
4. update replicas, if replicas are not '3' then update nodes in [redis-config]() configmap.

Apply all the files under redis-3.0.7 folder

```
kubectl apply -f redis-3.0.7/
```