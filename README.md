

# 🌟 CSS Exercise: Build a Responsive Navigation Layout

## Objective:
Create a responsive webpage with:

- A **horizontal navigation bar** at the top.
- A **vertical side menu** on the left.
- A **dropdown menu** inside the top navbar.
- Layout arranged with **Flexbox** and **CSS Grid**.

---

## Requirements:

### 1. Top Navigation Bar (Flexbox)

- Horizontally aligned at the top of the page.
- Contains:
  - Logo on the left.
  - Navigation links ("Home", "About", "Services", "Contact").
  - A "More" item with a **dropdown menu** showing "Blog", "Careers", "Help".

### 2. Vertical Sidebar (Flexbox/Grid)

- Fixed on the left side.
- Contains:
  - Links like "Dashboard", "Settings", "Profile", "Logout".
- Should be scrollable if content overflows.

### 3. Main Content Area (Grid)

- Next to the sidebar.
- Use **CSS Grid** to create:
  - A 2-column layout inside the main area (e.g., Articles and Widgets).

### 4. Styling:

- Use Flexbox for the navbar and sidebar.
- Use Grid for the main content area.
- Add basic hover effects for links.
- Make it responsive:
  - On smaller screens, collapse the sidebar and show a "menu" button instead.

---

## Files to create:

- `index.html`
- `style.css`

---

## Example starter HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Navigation Exercise</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <header class="navbar">
    <div class="logo">MyLogo</div>
    <nav class="nav-links">
      <a href="#">Home</a>
      <a href="#">About</a>
      <a href="#">Services</a>
      <a href="#">Contact</a>
      <div class="dropdown">
        <button class="dropbtn">More</button>
        <div class="dropdown-content">
          <a href="#">Blog</a>
          <a href="#">Careers</a>
          <a href="#">Help</a>
        </div>
      </div>
    </nav>
  </header>

  <div class="container">
    <aside class="sidebar">
      <a href="#">Dashboard</a>
      <a href="#">Settings</a>
      <a href="#">Profile</a>
      <a href="#">Logout</a>
    </aside>

    <main class="main-content">
      <section class="articles">
        <h2>Articles</h2>
        <!-- Articles here -->
      </section>
      <section class="widgets">
        <h2>Widgets</h2>
        <!-- Widgets here -->
      </section>
    </main>
  </div>

</body>
</html>
```

---

## Key CSS to Practice:

- Flexbox:
  - `display: flex`
  - `justify-content: space-between`
  - `align-items: center`
- Dropdown:
  - `position: relative`
  - `position: absolute`
  - `display: none` and `:hover`
- Grid:
  - `display: grid`
  - `grid-template-columns`
  - `gap`

