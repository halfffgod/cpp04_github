NAME		= animal
SRC			= main.cpp Animal.cpp Cat.cpp Dog.cpp WrongAnimal.cpp WrongCat.cpp Brain.cpp
OBJ			= main.o Animal.o Cat.o Dog.o WrongAnimal.o WrongCat.o Brain.o
CC			= g++
FLAGS		= -Wall -Wextra -Werror -std=c++98
RM			= rm -f
all:		$(NAME)

.cpp.o:
			@$(CC) $(FLAGS) -o $@ -c $<

$(NAME):	$(OBJ)
			@$(CC) $(FLAGS) -o $(NAME) $(OBJ)
			@echo "$(NAME) is compiled!"

clean:
			@$(RM) $(OBJ)

fclean:		clean
			@$(RM) $(NAME)

re:			fclean all

.PHONY:		all clean fclean re