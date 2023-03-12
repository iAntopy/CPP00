# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: iamongeo <iamongeo@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/03/16 20:27:40 by iamongeo          #+#    #+#              #
#    Updated: 2023/03/12 13:56:17 by iamongeo         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

SRCS	=	tests.cpp

CLS	=	Account.cpp

OBJS	=	$(SRCS:.cpp=.o) $(CLS:.cpp=.o)

CPPSTD	=	-std=c++98

CPPFLGS	=	$(CPPSTD) -Wall -Werror -Wextra

CPP	=	c++

NAME	=	Accounting

.c.o:
	$(CPP) $(CPPFLGS) -o $< -c $@

$(NAME):	$(OBJS)
	$(CPP) $(CPPFLGS) -o $(NAME) $(OBJS)

all:	$(NAME)

clean:
	rm $(OBJS)

fclean:	clean
	rm $(NAME)

re:	fclean all
