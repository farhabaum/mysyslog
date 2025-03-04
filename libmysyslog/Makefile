all:
  gcc -fPIC -shared -o libmysyslog-text.so libmysyslog-text.c
	gcc -fPIC -shared -o libmysyslog-json.so libmysyslog-json.c
	gcc -fPIC -shared -o libmysyslog.so libmysyslog.c -ldl
	gcc -o myapp mysyslog-client.c libmysyslog.so -ldl


clear:
	rm -rf *.so
