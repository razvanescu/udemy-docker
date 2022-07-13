# Udemy-Docker.and.Kubernetes.The.Complete.Guide

## Status
// 2022-05-15 - 001



` docker run hello-world `

` docker run image-name command `

### Commands
 1. docker run hellow-world 
 1. docker ps
 2. docker ls 
 --- 
 3. docker create hellow-world
 4. docker start -a [containnerID]
 // -a show the result to my terminal
 5. docker logs [containerID]
 ---
 6. docker stop [containerID]
 7. docker kill [containerID]

 ---
 8. docker exec -it [containerID] sh
 // start sh console on containner


## Redis Install

/usr/local/opt/redis/bin/redis-server 
/usr/local/etc/redis.conf


## 🍺 MacOs BREW Update

`
==> Installing node
==> Pouring node--18.0.0.big_sur.bottle.tar.gz
Error: The `brew link` step did not complete successfully
The formula built, but is not symlinked into /usr/local
Could not symlink bin/node
Target /usr/local/bin/node
already exists. You may want to remove it:
  rm '/usr/local/bin/node'

To force the link and overwrite all conflicting files:
  brew link --overwrite node

To list all files that would be deleted:
  brew link --overwrite --dry-run node`

  ---

  9.	docker build -t razvanescu/alipn-redis:latest
  // 037 Video
  10. 	docker commit -c 'CMD ["redis-server"]' [containerId]
  // 038 Video

  11. docker run -p 6000:8080 razvanescu/simpleweb //047
  ---

  ## docker-compose.yml

  101. docker-compose up
  102. docker-compose up -d
  103. docker-compose down
  104. docker-compose up --build

  ## Volumes

  200. docker build -f Dockerfile.dev -t razvanescu/[Project]:[tag] .   //DON'T FORGET about .
  201. docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app <image_id>
  
  ## Execute commands in containner

  202. docker run -it razvanescu/frontend npm run test
  203. 083 => 

  204. 093 => 