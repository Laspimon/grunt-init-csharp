
all: build.debug-quiet run.debug

build.release-quiet:
	@xbuild /p:Configuration=Release /verbosity:quiet /nologo  {%= name %}.csproj

build.debug-quiet:
	@xbuild /p:Configuration=Debug /verbosity:quiet /nologo {%= name %}.csproj

build.debug:
	@xbuild /p:Configuration=Debug /nologo {%= name %}.csproj

build.release:
	@xbuild /p:Configuration=Release /nologo {%= name %}.csproj

run.release:
	@xterm -e "mono bin/Release/{%= name %}.exe"

run.debug:
	@xterm -e "mono bin/Debug/{%= name %}.exe"

clean:
	@rm -rf ./bin/
	@echo "DEL BIN"
	@rm -rf ./obj/
	@echo "DEL OBJ"
