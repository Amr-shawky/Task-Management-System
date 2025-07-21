# ✅ Taskify - Task Management System

Taskify is a lightweight and extensible task management system built with **ASP.NET Core 8 Web API**. It allows users to organize tasks efficiently, collaborate through comments, and stay updated with notifications and reports.

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

- **.NET 8 (LTS)**
- **ASP.NET Core Web API**
- **Entity Framework Core**
- **Docker (Optional)**
- **C#**
- **LINQ**
- **MediatR** *(optional for CQRS pattern)*
- **BackgroundService / Hangfire** *(for background tasks)*
- **iTextSharp / QuestPDF** *(for PDF reports)*
- **MailKit / SMTP** *(for sending emails)*

---

## 🛠️ Setup Instructions

1. Clone the repository:
`` 
   git clone https://github.com/yourusername/taskify-api.git
`` 

2. Navigate to the project directory:

   `` 
   cd taskify-api
   `` 

3. Configure the `appsettings.json` with:

   * Database connection string
   * SMTP email credentials

4. Run database migrations:

   `` 
   dotnet ef database update
   `` 

5. Run the application:
   `` 
   dotnet run
   `` 
---

## 🐳 Docker Support

> If you selected Docker support during setup:

Build and run the container:
`` 
docker build -t taskify-api .
docker run -p 5000:80 taskify-api
`` 

---

## 📬 Email Notifications

Make sure to configure your SMTP settings under `appsettings.json` for email features to work properly.

---

## 📄 PDF Reports

Tasks marked as **completed** will be included in the downloadable PDF report. This can be generated manually or automatically via background jobs.

---

## 🧑‍💻 Author

**Amr Mohamed Shawky**
.NET Developer | Egypt
GitHub: [Amr-shawky](https://github.com/Amr-shawky)

