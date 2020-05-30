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

all: clean compile run

compile:
	@printf "Compilando arquivos..."
	@gcc -c $(SRC)/horas.c -I $(INCLUDE) -o $(OBJ)/horas.o
	@gcc -c $(SRC)/frase.c -I $(INCLUDE) -o $(OBJ)/frase.o
	@gcc $(APPS)/teste.c $(OBJ)/*.o -I $(INCLUDE) -o $(BIN)/teste.exe
	@printf "OK\n"
		
run:
	@printf "Executando a aplicação:\n"
	@printf "========================================\n"
	@echo
	@$(BIN)/teste.exe
	@echo
	@printf "========================================\n"
	@printf "Aplicação executada com sucesso!!\n\n"
	
clean:	
	@printf "\nLimpando compilações anteriores..."
	@rm $(OBJ)/*.o
	@rm $(BIN)/*
	@printf " OK\n"