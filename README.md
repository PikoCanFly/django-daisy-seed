# 🌱 Django + Tailwind CSS Starter Project (Daisy Seed)
A minimal, modern Django starter template using Tailwind CSS, DaisyUI components, and a persistent light/dark theme toggle.

---

# 🎥 Youtube:

Watch the step-by-step tutorial video/project demo:

[![Watch the video](https://img.youtube.com/vi/7qPaBR6JlQY/hqdefault.jpg)](https://youtu.be/7qPaBR6JlQY)

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

* Python 3.10+ (along withpip / uv)
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
   cd daisyseed
   python manage.py migrate
   ```

5. **Run the development server**

   ```bash
   python manage.py runserver
   ```   

# **Installing and configuring Tailwind CSS & DaisyUI**

6. **Open a new terminal & Install Tailwind CSS & DaisyUI**

   ```
   npm install
   ```



7. **Build CSS**

   ```
   npm run watch:css
   ```

## 🎥 Step-by-Step Installation & Setup Guide

Watch the full walkthrough here: [YouTube - Installation & Setup](https://m.youtube.com/watch?v=7qPaBR6JlQY&t=2308s)


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

## ⁉️ How to Change Project Name
The project name will be daisyseed. However, changing it to any name you want is a quick and easy process; as shown in the following tutorial:
[![Watch the video](https://img.youtube.com/vi/Ak4XA5QK3_w/hqdefault.jpg)](https://youtu.be/Ak4XA5QK3_w)


## 🤝 Support
If you find this project useful and want to support me:

- 🌟  Star this repo! 

- Subscribe to my YouTube channel: https://www.youtube.com/@PikoCanFly

- Become a channel member for exclusive content and support: https://www.youtube.com/channel/UC8NoIbiu78iGMnh_xezgx8A/join

- Give thanks directly on YouTube by clicking the "Thanks" button under my video

## 📄 License

MIT License © 2025 Piko Can Fly

