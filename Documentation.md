# Responsive Layout using Flexbox

This project demonstrates how to create a responsive web page layout using Flexbox. 
The layout is designed to adapt and look visually appealing across various screen sizes and devices.
## HTML Structure
```sh
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Responsive Layout</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header>
    <!-- Add your header content here -->
  </header>

  <nav>
    <!-- Add your navigation content here -->
  </nav>

  <main>
    <!-- Add your main content here -->
  </main>

  <aside>
    <!-- Add your sidebar content here -->
  </aside>

  <footer>
    <!-- Add your footer content here -->
  </footer>
</body>
</html>
```

## Flexbox Properties
## _Header_
In the header, display: flex sets it as a flex container, justify-content: space-between aligns the logo and navigation menu at the ends, 
and align-items: center vertically centers the content.
```sh
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #f0f0f0;
  padding: 10px;
}
```

## Navigation
For the navigation, we use display: flex to arrange the menu items horizontally, and margin-right creates space between each menu item.
```sh
nav ul {
  list-style: none;
  display: flex;
}

nav li {
  margin-right: 20px;
}
```

## Main Content and Sidebar
In the main section, we set display: flex to create a flex container, and .main-content is given flex: 1 to take up the available space,
while aside has a fixed width of 200px with flex: 0 0 200px.
```sh
main {
  display: flex;
  padding: 20px;
}

.main-content {
  flex: 1;
  margin-right: 20px;
}

aside {
  flex: 0 0 200px;
  min-width: 200px;
  padding: 20px;
  background-color: #f0f0f0;
}
```

## Footer
The footer is styled with background color, text color, centered text, and padding for spacing.
```sh
footer {
  background-color: #333;
  color: #fff;
  text-align: center;
  padding: 10px;
}
```

## Media Queries and Breakpoints
To make the layout responsive, media queries are introduced to adapt to different screen sizes:

| Device | Size |
| ------ | ------ |
| Tablets | max-width: 768px |
| Mobile | max-width: 480p |