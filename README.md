# Laravel 13 CRUD Demo — Simple Blog

A demo project for the tutorial **Laravel 13 CRUD: Build a Simple Blog Step by Step**.

📖 **Read the full tutorial at:** [qadrlabs.com/post/laravel-13-crud-tutorial-build-a-simple-blog-step-by-step](https://qadrlabs.com/post/laravel-13-crud-tutorial-build-a-simple-blog-step-by-step)

---

## About This Project

This is a simple blog application built with **Laravel 13** to demonstrate CRUD (Create, Read, Update, Delete) operations. It is designed for beginners who want to learn the fundamentals of web development with Laravel.

### Features

- ✅ List all posts (Read)
- ✅ Create a new post (Create)
- ✅ View post detail (Read)
- ✅ Edit a post (Update)
- ✅ Delete a post (Delete)
- ✅ Post status: `draft` / `publish`
- ✅ Auto-generated slug from post title

### Tech Stack

| Technology | Version |
|------------|---------|
| PHP | ^8.3 |
| Laravel | ^13.0 |
| Database | MySQL |
| Vite | (Frontend bundler) |

---

## Requirements

Before getting started, make sure you have the following installed:

- **PHP** >= 8.3
- **Composer** >= 2.x
- **Node.js** >= 18.x & **npm**
- **MySQL** >= 5.7 or MariaDB >= 10.3

---

## Setup Steps

### 1. Clone the Repository

```bash
git clone https://github.com/qadrLabs/laravel-13-crud-demo.git
cd laravel-13-crud-demo
```

### 2. Install PHP Dependencies

```bash
composer install
```

### 3. Copy the Environment File

```bash
cp .env.example .env
```

### 4. Generate Application Key

```bash
php artisan key:generate
```

### 5. Configure the Database

Open your `.env` file and update the database credentials:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

> Make sure the MySQL database already exists before running the migration.

### 6. Run Database Migration

```bash
php artisan migrate
```

### 7. Install JavaScript Dependencies

```bash
npm install
```

### 8. Build Frontend Assets

```bash
npm run build
```

### 9. Start the Development Server

```bash
php artisan serve
```

Or run all services at once (server, queue, logs, vite) using:

```bash
composer dev
```

The application will be available at: **http://localhost:8000**

---

## Running Tests

```bash
composer test
```

---

## Project Structure

```
laravel-13-crud-demo/
├── app/
│   ├── Http/
│   │   └── Controllers/
│   │       └── PostController.php   # CRUD Controller for Post
│   └── Models/
│       └── Post.php                 # Post Model
├── database/
│   └── migrations/
│       └── ..._create_posts_table.php  # Posts table schema
├── resources/
│   └── views/                       # Blade templates
├── routes/
│   └── web.php                      # Application routes
└── .env.example                     # Example environment configuration
```

---

## References

- 📖 [Full Tutorial](https://qadrlabs.com/post/laravel-13-crud-tutorial-build-a-simple-blog-step-by-step)
- 🐙 [GitHub Repository](https://github.com/qadrLabs/laravel-13-crud-demo)
- 📦 [Laravel Documentation](https://laravel.com/docs/13.x)

---

## License

This project is open-sourced under the [MIT License](https://opensource.org/licenses/MIT).
