
all: build.debug-quiet run.debug

build.release-quiet:
	@echo "make: build -release -quiet"
	@xbuild /p:Configuration=Release /verbosity:quiet /nologo  {%= name %}.csproj

build.debug-quiet:
	@echo "make: build -debug -quiet"
	@xbuild /p:Configuration=Debug /verbosity:quiet /nologo {%= name %}.csproj

build.debug:
	@echo "make: build -debug"
	@xbuild /p:Configuration=Debug /nologo {%= name %}.csproj

build.release:
	@echo "make: build -release"
	@xbuild /p:Configuration=Release /nologo {%= name %}.csproj

run.release:
	@echo "make: run -release"
	@xterm -bg black -fg white -geometry 100x55-0+0 -e "mono bin/Release/{%= name %}.exe"

run.debug:
	@echo "make: run -debug"
	@xterm -bg black -fg white -geometry 100x55-0+0 -e "mono bin/Debug/{%= name %}.exe"

profile:
	@echo "make: build -debug -quiet"
	@xbuild /p:Configuration=Debug /verbosity:quiet /nologo {%= name %}.csproj
	@echo "make: profile"
	@mono --profile=log:report,noalloc,nocalls bin/Debug/{%= name %}.exe

clean:
	@echo "make: clean"
	@rm -rf ./bin/
	@rm -rf ./obj/
