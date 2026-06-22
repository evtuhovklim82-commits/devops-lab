# 🖥️ DevOps мониторинг-стек (Pet-проект)

Этот проект — моя лабораторная среда для изучения системного администрирования и мониторинга. Я развернул полный цикл сбора метрик и оповещений с помощью Docker.

## 🚀 Стек технологий
- **ОС:** Arch Linux (установка с нуля, ручная настройка)
- **Контейнеризация:** Docker, Docker Compose
- **Мониторинг:** Prometheus (сбор метрик)
- **Визуализация:** Grafana (дашборды)
- **Оповещения:** Alertmanager (отправка уведомлений на почту)
- **Автоматизация:** Bash-скрипты, Systemd, Cron

## ⚡ Быстрый старт (как запустить)

```bash
git clone https://github.com/evtuhovklim82-commits/devops-lab.git
cd devops-lab
docker-compose up -d
После запуска сервисы будут доступны по адресам:

    Grafana: http://localhost:3000 (логин/пароль: admin/admin)

    Prometheus: http://localhost:9090

    Alertmanager: http://localhost:9093

📁 Структура проекта
.
├── configs/
│   ├── prometheus/
│   │   ├── prometheus.yml      # Конфиг сбора метрик
│   │   └── alerts.yml          # Правила для алертов (CPU, падения)
│   └── alertmanager/
│       └── alertmanager.yml    # Конфиг отправки писем и группировки
├── scripts/
│   ├── backup.sh               # Бэкап данных
│   └── cleanup.sh              # Очистка старых логов
├── systemd/
│   └── docker-services.service # Автозапуск при старте системы
└── docker-compose.yml
🔧 Что я умею (навыки, которые применил)

    Установка Arch Linux вручную (разбивка дисков, GRUB, сеть).

    Настройка пользовательских сетей в Docker.

    Написание Bash-скриптов для бэкапа и очистки диска.

    Создание Systemd-юнитов для автозапуска контейнеров.

    Настройка цепочки мониторинга: Метрика → Алерт → Оповещение на почту.

    Работа с Git (ветки, SSH-ключи, разрешение конфликтов).

📬 Контакты

    Email: clevis.bash@gmail.com

    GitHub: evtuhovklim82-commits
