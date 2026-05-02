# 🚀 API Wizards

<p align="center">
  <b>Production-ready FastAPI backend for a photo-sharing platform</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/FastAPI-async-green">
  <img src="https://img.shields.io/badge/PostgreSQL-db-blue">
  <img src="https://img.shields.io/badge/Docker-ready-blue">
  <img src="https://img.shields.io/badge/Python-3.11-blue">
</p>

---

## ⚡ About

**API Wizards** — це повноцінний backend сервіс, який демонструє реальну production-архітектуру:

* авторизація з JWT
* ролі користувачів
* робота з фото + трансформації
* масштабована структура (service / repository)

Це не просто pet-project — це **демонстрація рівня Junior+ / Middle backend developer**.

---

## 🧱 Tech Stack

* **FastAPI**
* **SQLAlchemy (async)**
* **PostgreSQL**
* **Alembic**
* **Docker Compose**
* **Redis (ready)**
* **Cloudinary**

---

## ✨ Features

### 🔐 Auth & Users

* Реєстрація / логін
* JWT (access + refresh)
* Email підтвердження
* Ролі: `admin`, `moderator`, `user`

### 🖼 Photos

* Завантаження фото
* Resize / crop / filters
* Форматування
* Text overlay
* Метадані

### 💬 Social

* Коментарі
* Теги

### ⚙️ System

* QR-коди
* Alembic міграції
* Swagger docs

---

## 📁 Architecture

```text
Client → FastAPI → Services → Repository → PostgreSQL
```

---

## 🚀 Quick Start

### 1. Clone

```bash
git clone https://github.com/AndreySamoylenko15/API_Wizards_.git
cd API_Wizards_
```

### 2. Env

```bash
cp .env.example .env
```

### 3. Run services

```bash
docker compose up -d
```

### 4. Install

```bash
python -m pip install -r requirements.txt
```

### 5. Migrations

```bash
python -m alembic upgrade head
```

### 6. Start API

```bash
python -m uvicorn main:app --reload
```

---

## 📚 API Docs

👉 http://127.0.0.1:8000/docs

---

## 🧪 Example Request

```bash
curl -X POST "http://127.0.0.1:8000/api/auth/signup" \
-H "Content-Type: application/json" \
-d '{"username":"andreydev","email":"andreydev@example.com","password":"password123"}'
```

---

## ⚠️ Notes

* Перший користувач → `admin`
* Потрібне підтвердження email
* Cloudinary потрібен для фото

---

## 🎯 What this project proves

* Вміння будувати backend-архітектуру
* Робота з async
* JWT + security flows
* Робота з медіа





---

⭐ Якщо проєкт корисний — постав зірку
