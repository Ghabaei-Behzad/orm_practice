Behzad Ghabaei <br>
CS 85 PHP programming <br>
Module 8 Assignment 8A <br>
Laravel with Database Environment <br>
Instructor Seno <br>
7/15/2026 <br>

### Set Up Instructions
#### How to configure a Laravel application to connect to a MySQL database using local tools.  Using XAMPP if on Windows. Verify the configuration by running a test migration and prepare the project to be shared via GitHub.
1. Use Xampp, Composer, VS Code, git, to create a Laravel project and connect it to a MySQL database <br>
2. Install Laravel globally, "composer global require laravel/installer" run this.  Type "laravel" to see if it is installed. <br>
3. Choose a folder that you want this project to be installed in, such as Documents/Development <br>
4. Create the project called orm_practice with the command "laravel new orm_practice" <br>
after the command: laravel new orm_practice <br>
Would you like to update now? No <br>
Which starter kit would you like to install? None <br>
Which testing framework do you prefer? Pest <br>
Do you want to install Laravel Boost to improve AI assisted coding? Yes <br>
Which database will our application use? mysql <br>
Default database updated. Would you like to run the default database migration? no <br>
Would you like to run npm install? no <br>
Which features would you like to configure? guidelines, skills,mcp <br>
Which integrations would you like to configure for Boost? None <br>
Which AI agents would you like to configure? GitHub Copilot <br>
cd orm_practice <br>
5. Change directory to it, run cd orm_practice. <br>
6. Open the project in VS Code. code . <br>
7. Launch the database using the XAMPP software, open the XAMPP Control Panel, start MySQL and Apache.  <br>
8. Open a browser and navigate to http://localhost/phpmyadmin <br>
9. Click "new" in the left sidebar and type in the "Table name" of the database. <br>
10. Name it "orm_practice_db" and click Create.<br>
11. To configure the Laravel .env file, set up the connection parameters inside the project settings.  Open VS Code (which should have your project loaded), and click on the .env file in the root folder <br>
12. Find this data base block and change it to this: <br>
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=orm_practice_db
DB_USERNAME=root
DB_PASSWORD=
```
13. Save the .env file. <br>
14. Now, run database migrations.  Create the default tables inside your newly created database,
with the command "php artisan migrate" <br>
15. Now, sanitize your environment variables: run "copy .env .env.example" in your terminal and type yes to overwrite. <br>
### Trouble Shooting Notes:
1. If the composer command is not found and if windows doesn't recognize composer, make sure you download and run the official Windows installer from GetComposer.org, then restart your terminal. <br>
2. If there is a XAMPP MySQL port conflict, and if MySQL fails to start, skype or another app might be using port 3306. Close those apps or change the port in XAMPP's config. <br>









<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

In addition, [Laracasts](https://laracasts.com) contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

You can also watch bite-sized lessons with real-world projects on [Laravel Learn](https://laravel.com/learn), where you will be guided through building a Laravel application from scratch while learning PHP fundamentals.

## Agentic Development

Laravel's predictable structure and conventions make it ideal for AI coding agents like Claude Code, Cursor, and GitHub Copilot. Install [Laravel Boost](https://laravel.com/docs/ai) to supercharge your AI workflow:

```bash
composer require laravel/boost --dev

php artisan boost:install
```

Boost provides your agent 15+ tools and skills that help agents build Laravel applications while following best practices.

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
