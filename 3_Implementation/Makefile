PROJ_NAME = bill
TEST_PROJ_NAME= Test_$(PROJ_NAME)

Build= build

SRC=src/ElectricityBill.c\
src/Information.c\
src/RuralArea.c\
src/UrbanArea.c\




INC= inc
INC_TEST= inc

TEST_SRC=unity_test/test.c\
unity_test/unity.c

ifdef OS
	RM=del
	FixPath=$(subst /,\,$1)
	EXEC=exe

else
	ifeq ($(shell uname),Linux)
		RM=rm -rf
		FixPath=$1
		EXEC=out
	endif

endif			

.PHONY: run clean test doc all

all:
	gcc -I $(INC) $(SRC)  -o $(call FixPath, $(PROJ_NAME).$(EXEC))


run:
	./$(call FixPath,$(PROJ_NAME).$(EXEC))


cppcheck:
	cppcheck --enable= all $(SRC) test.c

debug:
	gcc -I $(INC) $(SRC)  -g -o $(PROJ_NAME).$(EXEC)
	gdb $(PROJ_NAME).$(EXEC)

valgrind: all
	 valgrind ./$(call FixPath,$(PROJ_NAME).$(EXEC))	 


test:
	gcc -I $(INC) -I $(INC_TEST) $(TEST_SRC) $(SRC) -o $(call FixPath,$(TEST_PROJ_NAME).$(EXEC))
	./$(call FixPath,$(TEST_PROJ_NAME).$(EXEC))

clean:
	$(RM) $(call FixPath,*.out)