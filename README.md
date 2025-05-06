# Django + Tailwaind CSS Starter Project ( Daisy Seed )

A minimal, modern Django starter template using Tailwind CSS, DaisyUI components, and a persistent light/dark theme toggle.

---

## 🚀 Features

* **Home App**: A simple landing page displaying a welcome message.
* **Users App**: Custom user model (`CustomUser`) extending Django's `AbstractUser` for easy future customization.
* **Base Template**: `base.html` with reusable `content` and `scripts` blocks and linked Tailwind CSS.
* **Responsive Navbar**:

  * Home button (🏠)
  * Light/Dark theme toggle switch
* **Theme Toggle**:

  * Detects system preference on first load.
  * Saves user selection in `localStorage` for persistence.
  * Updates `<html data-theme="...">` to switch DaisyUI themes instantly.

## 📋 Prerequisites

* Python 3.8+
* Django 4.x
* Node.js & npm (for Tailwind CSS build)

## 🛠️ Installation

1. **Clone the repository**
⚠️ Note the . at the end



   ```
   git clone https://github.com/pikocanfly/django-daisy-seed.git .
   
   ```

2. **Create & activate a virtual environment**

   ```bash
   python -m venv venv
   venv/Scripts/activate  # On Linux/Mac OS use `source venv\bin\activate`
   ```

3. **Install Python dependencies**

   run:

     ```
     pip install -r requirements.txt
     ```
4. **Apply Migrations & Create Superuser**

   ```bash
   python manage.py migrate
   ```

5. **Run the development server**

   ```bash
   python manage.py runserver
   ```   

# **Installing and configuring Tailwind CSS & DaisyUI**

6. **Open a new terminal**

4. **Install Tailwind CSS & DaisyUI**

   ```
      npm install
   ```



6. **Build CSS**

   ```
   npm run watch:css
   ```



## ▶️ Usage

* Visit `http://127.0.0.1:8000/` to see the home page.
* Use the theme switcher in the navbar to toggle light/dark mode. Your choice will persist on reload.
* Access the Django admin at `/admin` to manage users via the custom user model.

## 🎨 How the Theme Toggle Works

1. On page load, a JavaScript script checks for a saved theme in `localStorage`.
2. If none is found, it falls back to the system preference via `window.matchMedia`.
3. The script sets the `<html data-theme="...">` attribute to either `light` or `dark`.
4. DaisyUI’s CSS responds to `data-theme` changes, automatically switching component styles.
5. The toggle input updates the attribute and saves the new theme back to `localStorage`.

## 🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request with improvements.

## 📄 License

MIT License © 2025 Piko Can Fly
# django-daisy-seed
