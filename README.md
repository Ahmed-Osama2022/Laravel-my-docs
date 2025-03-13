## php artisan commands I leaned till now:

---

### For stating the server:

- Regular one -> start with port 8000; and if it is reserved ; it will take 8001...
```bash
php artisan serve	
```
- To bind the app over the network
```bash
php artisan serve --host 0.0.0.0 
```
- To use a specific port
```bash
php artisan serve --port 3000
```
---

- To view all the routes available to your application:
```bash
  php artisan route:list
```

- To make a middleware:
```bash
php artisan make:middleware <MiddlewareName>
```

-  To view all the middleware available to your application:

  ```bash
  php artisan middleware:list
  ```

----

### Controllers

- To make a controller

  ```bash
  php artisan make:controller <controllerName>
  ```
- To make a Resource controller (Made for CRUD specifically)

```bash
php artisan make:controller -r <controllerName>
```

---

## Views

### Blade Template Engine

- To make a view (Blade Template Engine)

  ```bash
  php artisan make:view <viewname>
  ```

- To make a view (Blade Template Engine) and make it inside a directory

  You could use dot notation

```bash 
php artisan make:view <folderName.viewname>
```

- To load the views faster => You could precached first in the server in the path (storage/framework/views) using this command

  ```bash
  php artisan view:cache 
  ```


- Now  to cleat these files (cached views)

  ```bash
  php artisan view:clear
  ```

- To make an App Service Provider

```bash
php artisan make:provider <AppServiceProviderName>
```

---

### Blade Template Engine (Components)

- To make an anonymous (Regular) component.

```bash
php artisan make:component <ComponentName> --view
```

<p>This will make an anonymous component in /resources/views/</p>

- To make a class component  

```bash
php artisan make:component <ComponentName>
```

<p>This will make an class component in /App/View/Components/</p>

<p>And will make the component at /resources/views/</p>





