# Zabbix 7.4 + Grafana Monitoring Stack

Этот репозиторий содержит настройку Docker Compose для разворачивания мониторинговой системы с использованием Zabbix 7.4 и Grafana с установленным Zabbix-плагином.

## Компоненты
- Zabbix Server 7.4
- Zabbix Web Interface
- Zabbix Agent
- PostgreSQL
- Grafana с Zabbix-плагином

## Требования
- Docker
- Docker Compose

## Быстрый старт
1. Клонировать репозиторий
2. Настроить переменные в файле `.env` при необходимости
3. Запустить `docker-compose up -d`
4. Доступ к Zabbix: http://localhost:80 (Admin/zabbix)
5. Доступ к Grafana: http://localhost:3000 (admin/admin_password)

## Структура проекта
- `docker-compose.yml` - основной конфигурационный файл Docker Compose
- `.env` - файл с переменными окружения
- `grafana-provisioning/` - директория с файлами предварительной настройки Grafana

## Настройка интеграции
Grafana автоматически настраивается для работы с Zabbix через плагин alexanderzobnin-zabbix-app.
