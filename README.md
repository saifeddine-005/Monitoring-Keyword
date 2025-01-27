# Monitoring-Keyword
Keyword Monitor is a web application built with Laravel framework. It allows users to track the position of their website for specific keywords on search engines like Google. The application provides features such as:

screenshot

screenshot 1

screenshot 2

screenshot 3

screenshot 4

Features
Keyword management: Add, edit, and delete keywords to track.
Search engine selection: Choose the service to track (e.g., google.selenium, tools.seo.ai).
Position tracking: Monitor the position of your website for each keyword on the selected search engine.
Reporting: Generate reports to analyze the performance of your keywords over time.
User authentication: Secure access to the application with user registration and login.
Technologies Used
Laravel 11.9 as the backend framework
Vue.js 3 with Inertia.js for the frontend
Tailwind CSS for styling
Configuration files for Vite, Tailwind, and PHPUnit
Installation
Clone the repository: git clone https://github.com/yasinkuyu/keyword-monitor.git
Navigate to the project directory: cd keyword-monitor
Install dependencies: composer install and npm install
Copy the environment file: cp .env.example .env
Generate an application key: php artisan key:generate
Configure your database credentials in the .env file
Run database migrations: php artisan migrate
Start the development server: php artisan serve && npm run dev
Task Schedule
* * * * * /opt/homebrew/Cellar/php/8.3.6/bin/php /DEV/KeywordMonitor/artisan schedule:run >> /dev/null 2>&1

This cron job runs the schedule:run command every minute. This command will run any scheduled tasks that are defined in the App\Console\Kernel class. The >> /dev/null 2>&1 part of the command redirects the output of the command to the /dev/null file, which is a special file that discards all data written to it. This prevents the output of the command from being displayed in the terminal. If you encounter any router issues, run the php artisan ziggy:generate command.

Usage
Register a new account or log in with your existing credentials
Add keywords you want to track
Select the search engine for tracking
Monitor the position of your website for the added keywords
Generate reports to analyze the performance over time
Demo Data
php artisan migrate:rollback && php artisan migrate && php artisan db:seed
Demo data usage instructions:

You can restore, recreate, and add demo data to the database by running the above command.
These commands will delete all existing data in your database. So use them carefully.
Demo data can be used to test certain features of your application.
Learning Laravel
Laravel has the most extensive and thorough documentation and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the Laravel Bootcamp, where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, Laracasts can help. Laracasts contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.
