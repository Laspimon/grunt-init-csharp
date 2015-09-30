
all: build.debug-quiet run.debug

build.release-quiet:
	@xbuild /p:Configuration=Release /verbosity:quiet /nologo  test.csproj

build.debug-quiet:
	@xbuild /p:Configuration=Debug /verbosity:quiet /nologo test.csproj

build.debug:
	@xbuild /p:Configuration=Debug /nologo test.csproj

build.release:
	@xbuild /p:Configuration=Release /nologo test.csproj

run.release:
	@xterm -e "mono bin/Release/test.exe"

run.debug:
	@xterm -e "mono bin/Debug/test.exe"

clean:
	@rm -rf ./bin/
	@echo "DEL BIN"
	@rm -rf ./obj/
	@echo "DEL OBJ"
