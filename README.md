# Flask Wellness Web App 🐬✨

---

## Framework Used

- **Flask**
   A lightweight Python web framework for building simple web applications.
- **Bootstrap**
  For responsive design and styled components in the HTML templates.

---
## Pages Included

- 🏠 **Home Page**
  The initial landing page of the application. It features a friendly greeting that asks users “How are you feeling today?”, encouraging mindfulness and emotional awareness. Navigation links are available at the top via a soft-colored navbar.

- 📘 **About Page**
  Provides a concise description of the web application's purpose as a wellness check-in platform. The page includes styling that aligns with the app's soft and comforting design theme.

- 📩 **Contact Page**
 Features a functional contact form that allows users to input their name and a message. The form includes validation for required fields and uses styled input elements with rounded corners and soft hover effects for an enhanced user experience.

---

## How to Run the Project

1.  Clone or copy the project to your local machine.
2.  Open a terminal inside the project folder.
3.  Run the following command:

```bash
python3 app.py
```

or using Flask CLI:

```bash
export FLASK_APP=app.py
flask run --host=0.0.0.0 --port=5000
```
## Access the web app in your browser

```bash
http://<your-ip>:5000
```
Get your IP address using:

```bash
hostname -I
```

## Allow Port Through Firewall

```bash
sudo apt install ufw -y
sudo ufw allow 5000
```

---

## 🛠️ Issues Encountered and Solutions

### 1. Bootstrap Styles Not Applying Properly
- **Issue**: The design did not appear as expected when the web pages were first loaded.
- **Solution**: Ensured the correct Bootstrap CDN link was included in the `<head>` tag and placed custom styles after Bootstrap to avoid being overridden.

### 2. Contact Form Not Submitting
- **Issue**: The contact form did not show any response or message after submission.
- **Solution**: Verified that the form method was set to `POST`, and implemented basic Flask form handling logic inside `@app.route('/contact', methods=['GET', 'POST'])` in `app.py`.

### 3. Inaccessible Web App from Browser
- **Issue**: The Flask server worked in the terminal but could not be accessed from the host machine.
- **Solution**: Hosted the app on all interfaces using:
  ```bash
  export FLASK_APP=app.py
  flask run --host=0.0.0.0 --port=5000


