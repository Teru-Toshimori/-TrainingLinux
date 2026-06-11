CC = gcc
CFLAGS = -Wall -Wextra -g -O0 -MMD -MP
TARGET = calculator
SRCS = main.c calc.c
OBJS = $(SRCS:.c=.o)
DEPS = $(OBJS:.o=.d)

$(TARGET): $(OBJS)
	$(CC) $^ -o $@

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

-include $(DEPS)

.PHONY: clean
clean:
	rm -f $(TARGET) $(OBJS) $(DEPS)
