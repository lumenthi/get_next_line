# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: lumenthi <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2018/01/04 10:37:11 by lumenthi          #+#    #+#              #
#    Updated: 2018/01/04 11:08:02 by lumenthi         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

CC = gcc
INCLUDE = libft.h
FLAGS = -Werror -Wall -Wextra -Ilibft.h -c

NAME = libft.a

BLACK = '\033[30m'
GREEN = '\033[32m'
YELLOW = '\033[33m'
BLUE = '\033[34m'
MAGENTA = '\033[35m'
BLANK = '\033[0m'
CYAN = '\033[36m'
RED = '\033[31m'

SRCS = ft_atoi.c \
		ft_bzero.c \
		ft_isalnum.c \
		ft_isalpha.c \
		ft_isascii.c \
		ft_isdigit.c \
		ft_isprint.c \
		ft_itoa.c \
		ft_memalloc.c \
		ft_memccpy.c \
		ft_memchr.c \
		ft_memcmp.c \
		ft_memcpy.c \
		ft_memdel.c \
		ft_memmove.c \
		ft_memset.c \
		ft_putchar.c \
		ft_putchar_fd.c \
		ft_putendl.c \
		ft_putendl_fd.c \
		ft_putnbr.c \
		ft_putnbr_fd.c \
		ft_putstr.c \
		ft_putstr_fd.c \
		ft_strcat.c \
		ft_strchr.c \
		ft_strclr.c \
		ft_strcpy.c \
		ft_strdel.c \
		ft_strdup.c \
		ft_strequ.c \
		ft_striter.c \
		ft_striteri.c \
		ft_strjoin.c \
		ft_strlcat.c \
		ft_strlen.c \
		ft_strmap.c \
		ft_strmapi.c \
		ft_strncat.c \
		ft_strncpy.c \
		ft_strnequ.c \
		ft_strnew.c \
		ft_strnstr.c \
		ft_strrchr.c \
		ft_strsplit.c \
		ft_strstr.c \
		ft_strsub.c \
		ft_strtrim.c \
		ft_tolower.c \
		ft_toupper.c \
		ft_strcmp.c \
		ft_strncmp.c \
		ft_lstnew.c \
		ft_lstdelone.c \
		ft_lstdel.c \
		ft_lstadd.c \
		ft_lstiter.c \
		ft_lstmap.c \
		ft_power.c \
		ft_count_words.c \
		ft_sqrt.c \
		ft_intlen.c \
		ft_is_space.c \
		ft_realloc.c
OBJS = $(SRCS:.c=.o)

.PHONY: all clean fclean re

all: $(NAME)

$(NAME):
	@ $(CC) $(FLAGS) $(SRCS)
	@ ar rc $(NAME) $(OBJS)
	@ ranlib $(NAME)
	@ printf " ~ %b%b%b compiled!\n" $(GREEN) $(NAME) $(BLANK)

clean:
	@ printf " ~ Cleaning %bobject files%b...\n" $(YELLOW) $(BLANK)
	@ rm -f $(OBJS)

fclean: clean
	@ printf " ~ Cleaning %b%b%b...\n" $(RED) $(NAME) $(BLANK)
	@ rm -f $(NAME)

re: fclean all
