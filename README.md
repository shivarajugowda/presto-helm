# presto-helm
Presto related helm charts


# Install Redis

```
$ helm repo add bitnami https://charts.bitnami.com/bitnami
$ helm install redis bitnami/redis --set cluster.enabled=false
$ helm delete redis
```

# Install Benchto

```
$ helm install benchto ./benchto -f ./benchto_overrides.yaml
$ helm delete benchto
```

# Install Metastore

```
$ helm install metastore ./metastore -f ./metastore_overrides.yaml
$ helm delete metastore
```

# Install Presto
```
$ helm install presto ./presto -f ./presto-overrides.yaml
$ helm delete presto
```

# Install Redash
```
$ helm install redash redash/redash -f ./redash-overrides.yaml
```