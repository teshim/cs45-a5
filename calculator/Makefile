parts = main.o addition.o subtraction.o multiplication.o division.o

calculator: $(parts) operations.h
	cc -o calculator $(parts) operations.h

$(parts): %.o:%.c
	cc -c $< -o $@

clean:
	rm -f calculator $(parts)

.PHONY: clean
