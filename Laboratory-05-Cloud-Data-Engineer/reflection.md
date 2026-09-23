# Mission Reflection

Using object storage helped me understand why cloud storage works well for storing millions of photos. Object storage keeps each photo as an object with its own data and information. This makes large collections easier to organize compared to traditional block storage. Photos do not need to depend on a fixed disk structure, which makes object storage useful for handling many files.

Docker also made deploying the MinIO storage server easier. Instead of installing and configuring each component manually, I used a Docker container to run MinIO. The container provided the needed environment and made the setup simpler. I also learned how containers help keep applications organized and easier to manage.

A bucket is a storage container for objects. I think of a bucket as a folder for cloud files, although buckets have features designed for object storage. For example, I could create a bucket named “student-photos” and place my image files inside.

Large companies protect their object storage data by keeping copies on different servers and locations. They also use backups, replication, and redundant storage. If one physical server crashes, another copy helps keep the data available and prevents data loss.

My confidence in using the Linux command line is also growing. At first, I found commands confusing because I needed to remember the correct syntax and file locations. After practicing commands for Docker, folders, and MinIO, I became more comfortable using the terminal. I still need more practice, but I now feel more confident working with Linux commands and following cloud storage tasks.
