
all: build.debug-quiet

build.release-quiet:
	@echo "make: build release -quiet"
	@echo "make: run release"
	@xbuild /p:Configuration=Release /verbosity:quiet /nologo  {%= name %}.csproj

build.debug-quiet:
	@echo "make: build debug -quiet"
	@echo "make: run debug"
	@xbuild /p:Configuration=Debug /verbosity:quiet /nologo {%= name %}.csproj

build.debug:
	@echo "make: build debug"
	@echo "make: run debug"
	@xbuild /p:Configuration=Debug /nologo {%= name %}.csproj

build.release:
	@echo "make: build release"
	@echo "make: run release"
	@xbuild /p:Configuration=Release /nologo {%= name %}.csproj

clean:
	@echo "make: clean"
	@rm -rf ./bin/
	@rm -rf ./obj/
