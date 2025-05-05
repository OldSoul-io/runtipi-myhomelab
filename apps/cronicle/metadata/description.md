# Cronicle (Dockerized by Soulteary)

**Cronicle** is a multi-server task scheduler and runner, featuring a sleek web-based UI. It provides real-time monitoring, plugin support, and distributed job scheduling, making it an ideal replacement for traditional `cron`.

This RunTipi app uses the actively maintained [`soulteary/cronicle`](https://hub.docker.com/r/soulteary/cronicle) Docker image, pre-configured for easy self-hosting and secure reverse proxying via Traefik. It supports a clean local or remote domain setup with HTTPS, all managed directly from your Tipi dashboard.

> 🔐 **Default Credentials**
> - Username: `admin`
> - Password: `admin`

---

## 🔧 Key Features

- 🧠 Distributed multi-server architecture
- 🕒 Cron-like event scheduling with timezone support
- 👀 Real-time job output and system metrics
- 🔌 Plugin support (write in any language)
- 📈 Historical logging and performance graphs
- 🔑 API Keys and REST API for remote control
- 🌐 Traefik-ready for secure, routed access via `APP_DOMAIN` or `LOCAL_DOMAIN`

---

## 📚 Documentation

Learn more about Cronicle and how to build with it:

- 👉 [Setup Guide](https://github.com/jhuckaby/Cronicle/blob/master/docs/Setup.md)
- 👉 [Web UI Overview](https://github.com/jhuckaby/Cronicle/blob/master/docs/WebUI.md)
- 👉 [Plugin System](https://github.com/jhuckaby/Cronicle/blob/master/docs/Plugins.md)
- 👉 [REST API](https://github.com/jhuckaby/Cronicle/blob/master/docs/APIReference.md)

---

## 🧱 App Info

| Field        | Value                            |
|--------------|----------------------------------|
| Docker Image | `soulteary/cronicle:0.9.63`       |
| Source Code  | [GitHub](https://github.com/jhuckaby/Cronicle) |
| License      | MIT                              |
| Maintainer   | [@soulteary](https://github.com/soulteary) |
| App Type     | Automation, Scheduling           |

---

## 🖼 Screenshot

![Main Screenshot](https://pixlcore.com/software/cronicle/screenshots-new/job-details-complete.png)

---

## 🏢 Known Users

- Agnes & Dora
- Sling TV

---

## 🧾 Notes for Tipi Users

- RunTipi exposes Cronicle via both `APP_DOMAIN` and `cronicle.LOCAL_DOMAIN`.
- HTTPS is enabled by default using Tipi's Traefik + Certbot integration.
- Data is stored at `${APP_DATA_DIR}/data/*` — fully persistent across restarts.
- Configure timezone via the `TZ` environment variable (e.g., `America/New_York`).

---

## ⚖ License

Cronicle is licensed under the [MIT License](https://github.com/jhuckaby/Cronicle/blob/master/LICENSE), and this Docker image is distributed by [@soulteary](https://github.com/soulteary) under the same terms.