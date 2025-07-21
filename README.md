# Taskify - Task Management System

**Taskify** is a lightweight and extensible task management system built with **ASP.NET Core 8 Web API**.  
It allows users to organize tasks efficiently, collaborate through comments, and stay updated with notifications and reports.

---

## 🚀 Features

- 📝 Create, update, and delete tasks  
- 📌 Set priorities and deadlines  
- 👤 Assign tasks to users  
- 📬 Email notifications for:
  - New tasks  
  - Overdue tasks  
- 💬 Comment system for tasks  
- 📎 Upload and manage file/image attachments per task  
- 📊 Generate PDF reports for completed tasks  
- ⏰ Background jobs for automatic reminders  

---

## ⚙️ Tech Stack

- [.NET 8 (LTS)](https://dotnet.microsoft.com/en-us/)
- ASP.NET Core Web API  
- Entity Framework Core  
- C#  
- LINQ  
- BackgroundService (for background tasks)
- iTextSharp (for PDF reports)
- MailKit / SMTP (for sending emails)
- Docker (containerization and deployment)

## 🔄 Optional / Potential Enhancements

- MediatR (for implementing CQRS)
- Hangfire (for advanced background jobs)
- QuestPDF (alternative PDF generator)

---

## 🛠️ Setup Instructions

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/taskify-api.git
    ```

2. **Navigate to the project directory:**

    ```bash
    cd taskify-api
    ```

3. **Configure your `appsettings.json`:**

    - Database connection string  
    - SMTP email credentials  

4. **Run database migrations:**

    ```bash
    dotnet ef database update
    ```

5. **Run the application:**

    ```bash
    dotnet run
    ```

---

## 🐳 Docker Support

If you enabled Docker support during setup:

1. **Build the Docker image:**

    ```bash
    docker build -t taskify-api .
    ```

2. **Run the container:**

    ```bash
    docker run -p 5000:80 taskify-api
    ```

---

## 📬 Email Notifications

Make sure to configure the correct **SMTP settings** in `appsettings.json`  
for features like **new task emails** and **overdue reminders** to work properly.

---

## 📄 PDF Reports

Tasks marked as **completed** will be included in a **PDF report**.  
This can be generated **manually** or via **background jobs**.

---

## 🧑‍💻 Author

**Amr Mohamed Shawky**  
.NET Developer | Egypt  
GitHub: [Amr-shawky](https://github.com/Amr-shawky)
