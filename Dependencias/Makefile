# Makefile
# 
# Objetivo: Exemplo passo a passo da lógica dos arquivos Makefile.
#
# Versão 1.0
#
# Programador: Marcus Marinho Bezerra (marcusmarinhob) 29/05/2020
#
# Email: marcusmarinhob@gmail.com

all:
	@echo "INSTALAÇÃO DO GCC:"
	@echo "======================================="
	@sudo apt install gcc
	@echo
	@echo
	@echo "COMPILAÇÃO:"
	@echo "======================================="
	@echo "Compilando arquivo lib.c"
	@gcc -c lib.c -o lib.o
	@echo "Arquivo compilado com sucesso!"
	@echo
	@echo "Compilando arquivo main.c"
	@gcc main.c lib.o -o main.exe
	@echo "Arquivo compilado com sucesso!"
	@echo
	@echo	
	@echo "EXECUÇÃO:"
	@echo "======================================="
	@echo "Executando main.exe: "
	@echo
	@./main.exe


