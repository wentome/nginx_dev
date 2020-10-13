
default:	build

clean:
	rm -rf Makefile objs

build:
	$(MAKE) -f objs/Makefile

install:
	$(MAKE) -f objs/Makefile install

modules:
	$(MAKE) -f objs/Makefile modules

upgrade:
	/opt/soft/nginx/sbin/nginx -t

	kill -USR2 `cat /opt/soft/nginx/logs/nginx.pid`
	sleep 1
	test -f /opt/soft/nginx/logs/nginx.pid.oldbin

	kill -QUIT `cat /opt/soft/nginx/logs/nginx.pid.oldbin`
