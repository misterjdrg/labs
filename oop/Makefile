JAVA_SOURCES = $(wildcard src/**/*.java)
JAVA_CLASSES = $(patsubst src/%.java, target/%.class, $(JAVA_SOURCES))

build: target $(JAVA_CLASSES)


clean:
	rm -rf target

target:
	mkdir -p target

target/%.class: src/%.java
	javac -d target $<