# Install Tailwind CSS

- initialization.

```bash
npm init -y
```

- install.

```bash
npm install -D tailwindcss
```

- uninstall.

```bash
npm uninstall tailwindcss
```

- install with extensions postcss and autoprefixer.

```bash
npm install -D tailwindcss postcss autoprefixer
```

- add tailwind config.

```bash
npx tailwindcss init
```

# Configure your template paths

- add paths on **tailwind.config.js**.

```bash
content: ["./public/**/*.{html,js}"],
```

- add path on **package.json**

```bash
"dev":"npx tailwindcss -i ./src/css/input.css -o ./public/css/style.css --watch"
```

# Add the Tailwind directives to your CSS

- make file **input.css**.

- add @tailwind directives on **input.css** file.

```bash
@tailwind base;
@tailwind components;
@tailwind utilities;
```

# Start the Tailwind CLI build process

- build output

```bash
npx tailwindcss -i ./src/css/input.css -o ./public/css/style.css --watch
```

# Start using Tailwind in your HTML

```bash
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="/public/css/output.css">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```
