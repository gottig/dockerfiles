FROM php:7.2-cli

EXPOSE 8000
RUN mkdir /projdir
COPY index.php /projdir
WORKDIR /projdir
CMD ["php", "-S", "0.0.0.0:8000"]
