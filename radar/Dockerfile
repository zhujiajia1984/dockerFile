FROM node

# 项目目录
WORKDIR /home/node/radar

# 安装依赖包
RUN npm install -g cnpm --registry=https://registry.npm.taobao.org \
	&& cnpm install express-generator -g \
	&& cd .. && express --view=ejs -f radar \
	&& cd radar \
	&& cnpm install --save \
	&& cnpm install --save log4js \
	&& cnpm install --save moment \
	&& cnpm install --save redis \
	&& cnpm install --save mongodb \
	&& cnpm install --save jsonwebtoken \
	&& cnpm install --save cors
CMD ["npm", "start"]