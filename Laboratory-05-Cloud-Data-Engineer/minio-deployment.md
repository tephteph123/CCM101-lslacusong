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

The bucket created for the client is: client-photos

The client-photos bucket stores the sample file uploaded to the MinIO server.

## Environment Variables

The -e flags set environment variables for the MinIO container.

MINIO_ROOT_USER=cloudadmin sets the username used to log in to the MinIO Web Console.

MINIO_ROOT_PASSWORD=CloudNova2026! sets the password used to log in to the MinIO Web Console. These values provide the login credentials for the MinIO server.
