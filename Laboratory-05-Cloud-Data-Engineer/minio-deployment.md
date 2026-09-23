# MinIO Deployment

## Docker Command Used

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
```

This command runs the MinIO server using Docker.

## Port Used for Web Console

The MinIO Web Console uses port `9001`.

Port `9000` is used for the MinIO API.

## Bucket Created

The bucket created for the client is: `client-photos`

The `client-photos` bucket stores the uploaded sample file.

## Environment Variables

The MinIO container uses the following environment variables:

```bash
MINIO_ROOT_USER=cloudadmin
MINIO_ROOT_PASSWORD=CloudNova2026!
```

The username is `cloudadmin`, and the password is `CloudNova2026!`. These are used to log in to the MinIO Web Console.
