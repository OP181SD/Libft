# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: yasaidi <yasaidi@student.42.fr>            +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/11/29 16:22:33 by yasaidi           #+#    #+#              #
#    Updated: 2022/12/02 15:37:18 by yasaidi          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME	=	libft.a

SRCS	=	ft_isalpha.c \
			ft_isdigit.c \
			ft_isalnum.c \
			ft_isprint.c\
			ft_strnstr.c\
			ft_strlen.c \
			ft_memset.c \
			ft_isascii.c\
			ft_bzero.c \
			ft_memcpy.c\
			ft_memmove.c\
			ft_strlcpy.c\
			ft_strlcat.c\
			ft_toupper.c\
			ft_tolower.c\
			ft_strchr.c\
			ft_strrchr.c\
			ft_strncmp.c\
			ft_memchr.c\
			ft_memcmp.c\
			ft_atoi.c\
			ft_calloc.c\
			ft_strdup.c\
			ft_substr.c\
			ft_strjoin.c\
			ft_itoa.c\
			ft_split.c\
			ft_strmapi.c\
			ft_putchar_fd.c\
			ft_putstr_fd.c\
			ft_putnbr_fd.c\
			ft_strtrim.c\
			ft_striteri.c\
			ft_putendl_fd.c


OBJS	=	$(SRCS:.c=.o)

SRC_B	=	ft_lstadd_front.c \
			ft_lstsize.c \
			ft_lstnew.c\
			ft_lstlast.c \
			ft_lstadd_back.c\
			ft_lstdelone.c\
			ft_lstclear.c\
			ft_lstiter.c\
			ft_lstmap.c

OBJ_B	=	${SRC_B:.c=.o}

CFLAGS 	= -Wall -Wextra -Werror

CC		= cc

%.o: %.c
	${CC} ${CFLAGS} -c -I. $< -o $@

${NAME} : $(OBJS)
	ar rc  $(NAME) $(OBJS)

all		: ${NAME}

bonus	: ${OBJ_B}
	ar rv $(NAME) $(OBJ_B)

clean	:
	rm -f  $(OBJS) $(OBJ_B)

fclean	: clean
	rm -rf $(NAME)

re		:	fclean all


.PHONY: all clean fclean re bonus
