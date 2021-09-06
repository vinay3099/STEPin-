ifdef OS
   RM = del /q
   FixPath = $(subst /,\,$1)
   EXEC = exe
else
   ifeq ($(shell uname), Linux)
      RM = rm -rf
      FixPath = $1
	  EXEC = out -lm
   endif
endif

TEST_PROJ_NAME = Tic Tac Toe
BUILD_DIR=Build

INC =-Iinc 

SRC = src/check.c src/board.c src/rule.c 

PROJECT=main.c


	
execute:
	gcc $(INC) $(SRC) $(PROJECT) -o all.exe
run: execute
	./all.exe

