CC=gcc
CFLAGS=-I ../lib/

iaxvoipclient: iaxvoipclient.c
	$(CC) $(CFLAGS) iaxvoipclient.c  ../build/libiaxclient_lib.a -lm -pthread -lpulse-simple -lpulse -o iaxvoipclient
