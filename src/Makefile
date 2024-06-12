CC_FLAGS = -Wall -Wextra -Werror

all: s21_cat s21_grep create_ascii

s21_cat: cat/s21_cat.c cat/file_work.c cat/flags.c
	gcc $(CC_FLAGS) cat/s21_cat.c cat/file_work.c cat/flags.c -o s21_cat

s21_grep: grep/s21_grep.c grep/file_work.c grep/flags.c
	gcc $(CC_FLAGS) grep/s21_grep.c grep/file_work.c grep/flags.c -o s21_grep

create_ascii: create_ascii.c
	gcc $(CC_FLAGS) create_ascii.c -o create_ascii

clean:
	rm -rf s21_cat s21_grep create_ascii
	rm -f cat/*.o cat/*.gch grep/*.o grep/*.gch *.o *.gch

rebuild: clean all
