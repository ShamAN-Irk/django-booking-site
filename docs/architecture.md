# Архитектура проекта

## Общая схема

Проект построен как классическое Django-приложение, развернутое на Linux VPS.

Общая схема:

```text
Пользователь
   ↓
Домен / HTTPS
   ↓
Nginx
   ↓
Gunicorn
   ↓
Django application
   ↓
PostgreSQL