FROM alpine:3.8

RUN apk add php7-fpm

WORKDIR /var/www/html

#RUN set -ex \
#	&& cd /etc/php7 \
#	&& { \
#		echo '[global]'; \
#		echo 'error_log = /proc/self/fd/2'; \
#		echo; \
#		echo '[www]'; \
#		echo '; if we send this to /proc/self/fd/1, it never appears'; \
#		echo 'access.log = /proc/self/fd/2'; \
#		echo; \
#		echo 'clear_env = no'; \
#		echo; \
#		echo '; Ensure worker stdout and stderr are sent to the main error log.'; \
#		echo 'catch_workers_output = yes'; \
#	} | tee php-fpm.d/docker.conf \
#	&& { \
#		echo '[global]'; \
#		echo 'daemonize = no'; \
#		echo; \
#		echo '[www]'; \
#		echo 'listen = 9000'; \
#	} | tee php-fpm.d/zz-docker.conf

EXPOSE 9000

CMD ["php-fpm7"]

