NAME = libft.a

SRCS = ft_atoi.c ft_bzero.c ft_calloc.c ft_isalnum.c \
	ft_isalpha.c ft_isascii.c ft_isdigit.c ft_isprint.c \
	ft_memchr.c ft_memcmp.c ft_memcpy.c ft_memmove.c \
	ft_memset.c ft_strchr.c ft_strdup.c ft_strlcat.c \
	ft_strlcpy.c ft_strlen.c ft_strncmp.c ft_strnstr.c \
	ft_strrchr.c ft_tolower.c ft_toupper.c ft_substr.c \
	ft_strjoin.c ft_strtrim.c ft_split.c ft_itoa.c \
	ft_strmapi.c ft_striteri.c ft_putchar_fd.c ft_putstr_fd.c \
	ft_putendl_fd.c ft_putnbr_fd.c ft_putunbr_fd.c ft_putnbr_base.c\
	ft_putnbr_base_sc.c ft_count_num.c ft_count_num2.c ft_printf.c\
	ft_putadd_fd.c get_next_line.c get_next_line_utils.c\
	ft_strcmp.c ft_atol.c
	
BSRCS = ft_lstnew.c ft_lstadd_front.c ft_lstsize.c ft_lstlast.c \
	ft_lstadd_back.c ft_lstdelone.c ft_lstclear.c ft_lstiter.c \
	ft_lstmap.c 

OBJS = $(SRCS:.c=.o)

BOBJS = $(BSRCS:.c=.o)

#CFLAGS = -Wall -Werror -Wextra -g

HEADERS = libft.h

all: $(NAME)

$(NAME): $(OBJS) 
		ar rcs $(NAME) $(OBJS)

bonus: $(NAME) $(BOBJS) $(OBJS)
	ar rcs $(NAME) $(BOBJS)	

#$(BOBJS): $(BSRCS)
#	cc $(CFLAGS) -c $(BSRCS)

clean :
		rm -f $(OBJS) $(BOBJS)

fclean: clean
		rm -f $(NAME)

re: fclean all

.PHONY = fclean clean all bonus re
