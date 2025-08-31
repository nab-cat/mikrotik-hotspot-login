# 🔑 Custom HTML Login Page for MikroTik Hotspot

A fully customizable **HTML/CSS/JS login page** for MikroTik Hotspot, designed to replace the default MikroTik login template with a modern, user-friendly UI.

## 🚀 Features

* ✅ Clean and responsive design (works on desktop & mobile)
* ✅ Easy to customize (HTML, CSS, JS only)
* ✅ Plug-and-play with MikroTik Hotspot
* ✅ Supports logo, background, and custom branding
* ✅ Compatible with all MikroTik RouterOS Hotspot setups

---

## 📊 Comparison: Default vs Custom Login

| Feature             | MikroTik Default Login | Custom HTML Login              |
| ------------------- | ---------------------- | ------------------------------ |
| **Design**          | Very basic, outdated   | Modern, responsive, brandable  |
| **Customization**   | Limited (text only)    | Full control (HTML, CSS, JS)   |
| **User Experience** | Plain form, no styling | Interactive, better UI/UX      |
| **Mobile Friendly** | Not optimized          | 100% mobile-friendly           |
| **Branding**        | Cannot add easily      | Add logos, colors, backgrounds |

---

## ⚙️ Setup Guide

### 1. Prepare Files

1. Download or clone this repository.
2. Inside you’ll find files like:

   ```
   login.html
   logout.html
   md5.js
   style.css
   images/
   ```

### 2. Upload to MikroTik

1. Connect to your router via **Winbox / WebFig / FTP**.
2. Go to:

   ```
   Files → Drag & Drop all custom login files
   ```
3. Ensure all files are uploaded to the root `/hotspot/` directory.

### 3. Apply the Custom Login

1. Open **IP → Hotspot → Server Profiles**.
2. Edit your active Hotspot profile.
3. In the **HTML Directory** field, set it to:

   ```
   hotspot
   ```

   (or your chosen folder name).

### 4. Test

1. Connect a device to your Hotspot.
2. When redirected, you should now see the custom login page.
3. Try logging in with your Hotspot credentials.

---

## 🛠️ Customization

* Replace `logo.png` in `/images/` with your own logo.
* Edit `style.css` to match your brand colors.
* Modify `login.html` for extra fields, announcements, or terms & conditions.

---

## 📜 Notes

* Make sure `md5.js` is included — MikroTik uses MD5 hashing for login.
* File names must match the default MikroTik hotspot filenames (`login.html`, `logout.html`).
* Always keep a backup of the default login in case you need to revert.

---

## 📷 Screenshot (Optional)

*Add a screenshot here of your custom login page for better documentation.*

---

## 🤝 Contributing

Pull requests and improvements are welcome.

---

## 📄 License

MIT License – free to use and modify.

---

👉 Do you want me to also write a **short troubleshooting section** (like "why login page not showing" / "stuck on redirect") in case users face issues, or keep it clean and simple?
