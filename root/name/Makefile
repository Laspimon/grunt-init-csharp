
all:
	@xbuild /p:Configuration=Debug /verbosity:quiet /nologo {%= name %}.csproj
	@konsole --nofork -e "mono bin/Debug/{%= name %}.exe"
	@echo ""

.PHONY: release
release:
	@xbuild /p:Configuration=Release /verbosity:quiet /nologo  {%= name %}.csproj
	@konsole --nofork -e "mono bin/Release/{%= name %}.exe"
	@echo ""

.PHONY: debug
debug:
	@xbuild /p:Configuration=Debug /nologo {%= name %}.csproj
	@konsole --nofork -e "mono bin/Debug/{%= name %}.exe"
	@echo ""

.PHONY: build.debug
build.debug:
	@xbuild /p:Configuration=Debug /nologo {%= name %}.csproj
	@echo ""

.PHONY: build.release
	@xbuild /p:Configuration=Release /nologo {%= name %}.csproj
	@echo ""

.PHONY: clean
clean:
	@rm -rf ./bin/
	@echo "DEL BIN"
	@rm -rf ./obj/
	@echo "DEL OBJ"
