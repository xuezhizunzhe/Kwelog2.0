项目部署
项目使用 docker-compose 一键部署运行。

./config/config.docker.toml 是部署时读取的配置文件，其中有些变量会由 docker-compose 中的环境变量覆盖

具体可参考 deploy/start/docker-compose.yml

配置文件读取值的优先级: 环境变量 > config.docker.toml 中的值，因此使用 docker-compose 运行时，修改其中的 environment 即可。
