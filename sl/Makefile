prueba: prueba.c libcarteles.so
	gcc -o prueba prueba.c -L. -lcarteles

libcarteles.so: carteles.c
	gcc -shared carteles.c -o libcarteles.so

clean: 
	rm -f *.o *.so prueba main

all: prueba libcarteles.so
	
install: prueba libcarteles.so
	cp prueba /usr/local/bin
	cp libcarteles.so /usr/local/lib
