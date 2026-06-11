CC = gcc
CFLAGS = -Wall -Wextra -g -O0
TARGET = calculator
OBJS = main.o calc.o

$(TARGET): $(OBJS)
	$(CC) $^ -o $@

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

.PHONY: clean
clean:
	rm -f $(TARGET) $(OBJS)
