# React from scratch — dummy API

This laravel app is used to provide a few simple API endpoints for the React from scratch Laracasts series.

https://laracasts.com/series/react-from-scratch

There is no authentication nor access restriction in there — it's just meant to be ran locally alongside the React app to have some endpoints to hit.

For things to work properly, you'll need to:

-   **Seed the data**: Run the Database seeder with `php artisan migrate:fresh --seed`. You should see 9 puppies in your database.
-   **Create a symbolic link from source directory**: Run `php artisan storage:link` to make stored images accessible publicly.
-   **Run the Laravel app locally** and make sure the React app uses the correct API URL when trying to hit it.

# Starting this project

## API app

### Start the server

The `export` line sets PHP 8.4 for the current terminal session only.

```bash
cd ~/projects/react-from-scratch-api
export PATH="/opt/homebrew/opt/php@8.4/bin:$PATH"
php artisan serve
```

### View the API in the browser

http://127.0.0.1:8000/api/puppies

### View the database

Run in terminal:

```bash
open database/database.sqlite
```

#### Example: updating the database

- Add a new row to the `puppy_user` table
- Save with `CMD + S`

![Updating a liked puppy in the database](<Screenshot 2026-11-25 at 13.33.51.png>)

## React app

Repo: https://github.com/Dec-246/React-from-scratch

### Start the server

```bash
cd ~/projects/React-from-scratch
npm run dev
```
