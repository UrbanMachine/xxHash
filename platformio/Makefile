all: include_dir src_dir others

include_dir:
	mkdir -p build/include
	cp ../xxhash.h ../xxh3.h build/include/

src_dir:
	mkdir -p build/src
	cp ../xxhash.c build/src/

others:
	mkdir -p build
	cp library.json ../README.md ../LICENSE build/

publish:
	pio pkg publish --owner urban-machine --type library build

clean:
	rm -rf build
