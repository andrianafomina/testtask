FROM nginx:alpine

# Удаляем дефолтную конфигурацию
RUN rm /etc/nginx/conf.d/default.conf

# Копируем кастомную конфигурацию
COPY nginx.conf /etc/nginx/conf.d/

# Создаем директорию для кастомных страниц ошибок
RUN mkdir -p /usr/share/nginx/errors

# Копируем страницу 500 ошибки
COPY 500.html /usr/share/nginx/errors/

# Открываем порт 80
EXPOSE 80

# Запускаем nginx
CMD ["nginx", "-g", "daemon off;"]
