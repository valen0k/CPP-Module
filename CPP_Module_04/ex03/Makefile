NAME =		Poly

SRC =		main.cpp AMateria.cpp Character.cpp Cure.cpp Ice.cpp MateriaSource.cpp

FLAGS =		-Wall -Werror -Wextra

OBJ = 		$(SRC:%.cpp=%.o)

.PHONY: all clean fclean re

all: $(NAME)

%.o: %.cpp
	clang++ $(FLAGS) -c $< -o $@

$(NAME): $(OBJ)
	clang++ $(FLAGS) $(OBJ) -o $(NAME)

clean:
	rm -rf $(OBJ)

fclean: clean
	rm -rf $(NAME)

re: fclean all

test: re
	./$(NAME)

de:
	clang++ -g $(SRC)
