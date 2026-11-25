# React from scratch — dummy API

This laravel app is used to provide a few simple API endpoints for the React from scratch Laracasts series.

There is no authentication nor access restriction in there — it's just meant to be ran locally alongside the React app to have some endpoints to hit.

For things to work properly, you'll need to:

-   **Seed the data**: Run the Database seeder with `php artisan migrate:fresh --seed`. You should see 9 puppies in your database.
-   **Create a symbolic link from source directory**: Run `php artisan storage:link` to make stored images accessible publicly.
-   **Run the Laravel app locally** and make sure the React app uses the correct API URL when trying to hit it.

# STARTING THIS PROJECT

## API APP

This will install PHP 8.4.x for the terminal session open and no longer after that.

use in terminal:

``` 
cd ~/projects/react-from-scratch-api
export PATH="/opt/homebrew/opt/php@8.4/bin:$PATH"
php artisan serve 
```

### React App

``` 
cd ~/projects/React-from-scratch
npm run dev 
```


# OPENING API in Browser

http://127.0.0.1:8000/api/puppies
