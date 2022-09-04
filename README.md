# 使用docker 运行
# 本地安装docker
# 该 vuepress 需要低版本 node 所以 通过docker运行更方便
docker run -it -d --name my_vuepress_blog --privileged -p 8081:8080 -v E:\junyi\study\my_vuepress_blog:/app/vue node:12.22.6 /bin/bash -c "cd /app/vue && node -v && npm config set registry https://registry.npm.taobao.org && npm install -D vuepress && npm run dev"