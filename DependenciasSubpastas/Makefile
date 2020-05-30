# Makefile
# 
# Objetivo: Exemplo passo a passo da lógica dos arquivos Makefile.
#
# Versão 1.0
#
# Programador: Marcus Marinho Bezerra (marcusmarinhob) 29/05/2020
#
# Email: marcusmarinhob@gmail.com

all: clean compile run

compile:
	@printf "Compilando arquivos..."
	@gcc -c ./src/horas.c -I ./include -o ./obj/horas.o
	@gcc -c ./src/frase.c -I ./include -o ./obj/frase.o
	@gcc ./apps/teste.c ./obj/*.o -I ./include -o ./bin/teste.exe
	@printf "OK\n"
		
run:
	@printf "Executando a aplicação:\n"
	@printf "========================================\n"
	@echo
	@./bin/teste.exe
	@echo
	@printf "========================================\n"
	@printf "Aplicação executada com sucesso!!\n\n"
	
clean:	
	@printf "\nLimpando compilações anteriores..."
	@rm ./obj/*.o
	@printf " OK\n"