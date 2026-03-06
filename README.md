CA1 - MySQL Docker Project

This project demonstrates how to create and manage a MySQL container using Docker and push the image to GitHub Container Registry (GHCR).

Steps Performed
1. Create Project Folder
mkdir ca_1
cd ca_1
2. Create Dockerfile
touch Dockerfile
nano Dockerfile
3. Build Docker Image
docker build -t sql_1612.
4. Run MySQL Container
docker run -d -p 3306:3306 sql_1612
5. Verify Running Container
docker ps
7. Login to GitHub Container Registry
docker login ghcr.io
8. Tag Docker Image
docker tag sql_1612 ghcr.io/ahrefdisha/sql_1612:v1
9. Push Image to GHCR
docker push ghcr.io/ahrefdisha/sql_1612:v1
10. Delete Image from Host Machine
docker rmi ghcr.io/ahrefdisha/sql_1612:v1
11. Pull Image Again from GHCR
docker pull ghcr.io/ahrefdisha/sql_1612:v1
Technologies Used
Docker
MySQL
GitHub Container Registry
