FROM node

# 项目目录
WORKDIR /home/node/myapp

# 安装依赖包
RUN mkdir bin && mkdir logs \
	&& npm install log4js@2.5.3 \
	&& npm install redis \
	&& npm install mongodb
CMD ["node", "/home/node/myapp/bin/token.js"]