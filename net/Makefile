PROGRAM = libWildcatNetworking.so
OBJECTS = networking.o http.o

libWildcatNetworking: $(OBJECTS)
	clang -shared -o $(PROGRAM) $(OBJECTS)

%.o: %.c
	clang -g -fPIC -c -o $@ -I. $<

clean:
	rm -f *.o libWildcatNetworking.so
