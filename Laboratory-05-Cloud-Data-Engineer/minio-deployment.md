# MinIO Deployment

## Docker Command Used

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
```

This Docker command deploys the MinIO server inside a Docker container. It also sets the ports and login credentials needed to access the MinIO Web Console.

## Port Used for Web Console

The MinIO Web Console uses port 9001. I used this port to access the MinIO Web Console through a web browser.

## Bucket Created

The bucket created for the client is: `client-photos`

The `client-photos` bucket is used to store the uploaded sample file.

## Environment Variables

The `-e` flags were used to set the environment variables for the MinIO server.

`MINIO_ROOT_USER=cloudadmin` sets the username for the MinIO Web Console.

`MINIO_ROOT_PASSWORD=CloudNova2026!` sets the password for the MinIO Web Console.
