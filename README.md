#!/bin/bash

# Укажи IP-адрес и порт прокси-сервера
PROXY_IP="192.168.1.1"
PROXY_PORT="8080"

# Настраиваем переменные окружения для использования прокси
export http_proxy="http://${PROXY_IP}:${PROXY_PORT}"
export https_proxy="http://${PROXY_IP}:${PROXY_PORT}"

# Для проверки выведем установленные значения прокси
echo "HTTP Proxy: $http_proxy"
echo "HTTPS Proxy: $https_proxy"
