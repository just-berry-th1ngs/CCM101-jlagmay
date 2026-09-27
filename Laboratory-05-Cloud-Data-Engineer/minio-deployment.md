
# MinIO Deployment Documentation

## Docker Command Used

Note: The official `minio/minio` image was discontinued from Docker Hub in October 2025, 
so this deployment uses the community-maintained `tobi312/minio` image instead, which uses 
the same environment variables and command structure.

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
tobi312/minio:latest server --console-address ":9001" /data
```

## Access Port

The MinIO Web Console was accessed via **port 9001** using the KillerCoda playground's port-forwarding feature.

## Bucket Created

- **Bucket name:** `client-photos`
- A sample file was uploaded to the bucket to confirm the storage server was functioning correctly.

## Environment Variables (-e flags) Explanation

- `MINIO_ROOT_USER` — sets the admin username used to log into the MinIO server and web console.
- `MINIO_ROOT_PASSWORD` — sets the admin password paired with the root user for authentication.

These flags configure the initial root credentials at container startup, similar to setting a default admin account for a new server.
