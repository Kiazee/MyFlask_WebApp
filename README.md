# Flask Wellness Web App 🐬✨

---

## Framework Used

- **Flask**
   A lightweight Python web framework for building simple web applications.
- **Bootstrap**
  For responsive design and styled components in the HTML templates.

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

