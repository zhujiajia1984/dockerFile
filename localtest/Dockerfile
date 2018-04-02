FROM node

# 项目目录
WORKDIR /home/node/myapp

# 安装依赖包
RUN npm install -g cnpm --registry=https://registry.npm.taobao.org \
	&& cnpm install express-generator -g \
	&& cd .. && express --view=ejs -f myapp \
	&& cd myapp \
	&& cnpm install --save body-parser@1.18.2 \
	&& cnpm install --save cookie-parser@1.4.3 \
	&& cnpm install --save cors@2.8.4 \
	&& cnpm install --save debug@2.6.9 \
	&& cnpm install --save ejs@2.5.7 \
	&& cnpm install --save express@4.15.5 \
	&& cnpm install --save log4js@2.5.3 \
	&& cnpm install --save moment@2.20.1 \
	&& cnpm install --save morgan@1.9.0 \
	&& cnpm install --save serve-favicon@2.4.5 \
	&& cnpm install --save redis \
	&& cnpm install --save mongodb \
	&& cnpm install jsonwebtoken
CMD ["npm", "start"]