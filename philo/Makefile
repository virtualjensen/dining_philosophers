# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: jebucoy <jebucoy@student.42abudhabi.ae>    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/04/10 16:41:43 by jebucoy           #+#    #+#              #
#    Updated: 2023/08/17 21:17:01 by jebucoy          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME	= philo

HEADER	=	./include

CC	=	cc

CFLAGS	=	-Wall -Wextra -Werror  -g3 -I $(HEADER) -pthread #-fsanitize=address

SRCS	=	main.c \
			parsing.c \
			init.c	\
			routine.c \
			utils.c \
			log_msg.c \
			clean.c \
			forks.c \

OBJS	= $(SRCS:.c=.o)

$(NAME)	:	$(OBJS)
		$(CC) $(CFLAGS) $(OBJS) -o $(NAME)

all	:	$(NAME)

clean	:
		rm -rf $(OBJS)

fclean	:	clean
		rm -rf $(NAME)

re	: fclean all