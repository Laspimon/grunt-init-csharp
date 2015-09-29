
all:
	@xbuild /p:Configuration=Release /verbosity:quiet /nologo {%= name %}.csproj
	@konsole --separate -e mono bin/Release/{%= name %}.exe
	@echo ""

.PHONY: debug
debug:
	@xbuild /p:Configuration=Debug /nologo  {%= name %}.csproj
	@konsole --separate -e mono bin/Debug/{%= name %}.exe
	@echo ""

.PHONY: run
run:
	@konsole --separate -e mono bin/Release/{%= name %}.exe
	@echo ""

.PHONY: clean
clean:
	@rm -rf ./bin/
	@echo "DEL BIN"
	@rm -rf ./obj/
	@echo "DEL OBJ"
