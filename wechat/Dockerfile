FROM node

# 项目目录
WORKDIR /home/node/wechat

# 安装依赖包
RUN apt-get update \
	&& apt-get install -y python-dev \
	&& curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py \
	&& python get-pip.py \
	&& pip install pycrypto \
	&& pip install redis \
	&& npm install -g cnpm --registry=https://registry.npm.taobao.org \
	&& cnpm install express-generator -g \
	&& cd .. && express --view=ejs -f wechat \
	&& cd wechat \
	&& cnpm install \
	&& cnpm install --save xml2js \
	&& cnpm install --save log4js \
	&& cnpm install --save moment \
	&& cnpm install --save redis \
	&& cnpm install --save mongodb \
	&& cnpm install --save jsonwebtoken \
	&& cnpm install --save cors
CMD ["npm", "start"]