FROM node

# 项目目录
WORKDIR /home/node/myapp

# 安装依赖包
RUN npm install -g cnpm --registry=https://registry.npm.taobao.org \
	&& cnpm install node-gyp -g \
	&& cnpm install ccap \
	&& cnpm install body-parser@1.18.2 \
	&& cnpm install cookie-parser@1.4.3 \
	&& cnpm install cors@2.8.4 \
	&& cnpm install debug@2.6.9 \
	&& cnpm install ejs@2.5.7 \
	&& cnpm install express@4.15.5 \
	&& cnpm install formidable@1.1.1 \
	&& cnpm install htmlparser2@3.9.2 \
	&& cnpm install log4js@2.5.3 \
	&& cnpm install moment@2.20.1 \
	&& cnpm install morgan@1.9.0 \
	&& cnpm install serve-favicon@2.4.5 \
	&& cnpm install xml-mapping@1.7.1 \
	&& cnpm install xmlreader@0.2.3 \
	&& cnpm install redis \
	&& cnpm install express-generator -g \
	&& cd .. && express --view=ejs -f myapp \
	&& cd myapp
CMD ["npm", "start"]