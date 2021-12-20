all: comp1.exe
comp1.exe: main.o func1.o func2.1.o
	gcc main.c func1.c func2.1.c -o comp1.exe
main.o: ../src/main.c
	gcc ../src/main.c -c -o main.o
func1.o: ../src/func1.c 
	gcc ../src/func1.c -c -o func1.o
func2.1.o: ../src/func2.1.c
	gcc ../src/func2.1.c -c -o func2.1.o
install: comp1.exe
	install ./comp1.exe/usr/local/bin
uninstall:
	rm /usr/local/bin/comp1.exe
clear:
	rm *.o comp1.exe
