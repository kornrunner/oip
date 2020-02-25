LDFLAGS= -lcryptopp -lSDL -lSDL_image -lpcap `pkg-config --libs freetype2`
CPPFLAGS = -g `pkg-config --cflags freetype2`

widgets = font.o widget.o label.o ../image.o textbox.o layout.o button.o option.o

guitest: ${widgets} guitest.o
	g++ ${LDFLAGS} ${widgets} guitest.o -o guitest
clean:
	rm -f *.o


