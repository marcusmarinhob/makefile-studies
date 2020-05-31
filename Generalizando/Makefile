# Makefile
# 
# Objetivo: Exemplo passo a passo da lógica dos arquivos Makefile.
#
# Versão 1.0
#
# Programador: Marcus Marinho Bezerra (marcusmarinhob) 29/05/2020
#
# Email: marcusmarinhob@gmail.com

APPS    = ./apps
BIN     = ./bin
INCLUDE = ./include
OBJ     = ./obj
SRC     = ./src

FLAGS = -O3 -Wall -std=gnu99

all: clean libed app run

libed: \
	$(OBJ)/horas.o \
	$(OBJ)/frase.o

app: $(BIN)/teste

$(OBJ)/%.o: $(SRC)/%.c $(INCLUDE)/%.h
	@printf "Compilando lib $@..."
	@gcc -c $< -I $(INCLUDE) $(FLAGS) -o $@
	@printf "OK\n"

$(BIN)/%: $(APPS)/%.c
	@printf "Compilando app $@.exe..."
	@gcc $< $(OBJ)/*.o -I $(INCLUDE) $(FLAGS) -o $@
	@printf "OK\n"	
		
run:
	@printf "Executando a aplicação:\n"
	@printf "========================================\n"
	@echo
	@$(BIN)/teste
	@echo
	@printf "========================================\n"
	@printf "Aplicação executada com sucesso!!\n\n"
	
clean:	
	@printf "\nLimpando compilações anteriores..."
	@rm $(OBJ)/*.o
	@rm $(BIN)/*
	@printf " OK\n"