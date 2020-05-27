FROM nginx:latest

COPY . /etc/nginx/.

RUN rm /etc/nginx/conf.d/default.conf
RUN mkdir /etc/nginx/sites-enabled/
RUN ln -s /etc/nginx/sites-available/localhost.conf /etc/nginx/sites-enabled/localhost.conf
