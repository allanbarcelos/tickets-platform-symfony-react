# Tickets Platform - Symphony PHP

This repository contains the updated version of a ticketing application originally developed in 2016, using **Symfony** for the backend and a **frontend without frameworks**, utilizing **jQuery** as the JavaScript library. The legacy code has been improved and restructured to provide a more robust and scalable platform.

## Repository Structure

```bash
/tickets-platform
├── /api           ← Symfony (PHP Backend)
│   └── ...
├── /app           ← Next.js (React Frontend)
│   └── ...
├── docker-compose.yml
├── .env
└── README.md
```

## About the Update

The updated version of the application underwent several improvements and restructuring, including:

- **Backend:** Symfony was maintained for the backend, but with performance improvements and code restructuring.
- **Frontend:** The frontend was completely revamped using **Next.js** (React), offering a more modern and responsive user experience.
- **Docker:** The application now uses **Docker** to separate services into containers, simplifying management and scalability.

## Legacy Application

The original code, developed in 2016, is still in production today. However, due to security reasons and sensitive data, the repository of the original version is private. If you're curious to explore the legacy code, please contact me, and I can provide access with certain limitations.

## Running the Project

### Prerequisites

Make sure you have the following tools installed:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

### Start the Containers

To run the application locally using Docker, follow these steps:

1. Clone the repository:
   ```bash
   git clone <Repository URL>
   cd tickets-platform
   ```

2. Build and start the containers:
   ```bash
   docker-compose up --build
   ```

3. Access the backend and frontend in your browser:

   - **Frontend (Next.js):** `http://localhost:3000`
   - **Backend (Symfony):** `http://localhost:8000`

## Contributing

Feel free to contribute with improvements or bug fixes! If you have suggestions or issues, please open an **issue** or submit a **pull request**.

---

**Note:** This project is an update of a legacy system and has some limitations, especially related to the original code. If you have any questions or need further clarification, feel free to reach out!