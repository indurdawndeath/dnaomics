# tlsvld Makefile
# AUTHORS:
#   - P. Christoph Champ
#   - Frank Zucker
#   - Ethan A. Merritt
TARGET  = tlsvld.so
F2PY    = f2py
FLAGS   = -c -m --opt=-O0
SOURCE  = tlsvld.f
OBJ     = tlsvld
#DEST    = /usr/lib64/python2.5/site-packages/mmLib/
DEST	= /usr/local/lib/python2.7/dist-packages/mmLib/

all: $(TARGET)

#$(TARGET): $(OBJ)
#        $(CC) -shared $(CLFAGS) -o $(TARGET) $(OBJ) $(LFLAGS)

$(TARGET):
	$(F2PY) $(FLAGS) $(OBJ) $(SOURCE)

install:
	cp $(TARGET) $(DEST)

clean:
	rm -f $(TARGET)
