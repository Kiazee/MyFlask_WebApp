# MyFlask_WebApp
# Flask Wellness Web App 

##  Framework Used
This project is built using **Flask**, a lightweight Python web framework that makes it easy to develop simple web applications quickly.

---

##  How to Run the Project

### 1. Clone or Download the Project
If cloned via Git:
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Or if downloaded as a .zip, extract it and cd into the project folder.

2. (Optional) Create a Virtual Environment
bash
Copy
Edit
python3 -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
3. Install Flask
bash
Copy
Edit
pip install flask
4. Run the Flask Server
bash
Copy
Edit
python app.py
5. Open in Browser
Visit http://localhost:5000 (or http://<VM_IP>:5000 from your host machine if running in VirtualBox).

🌟 Features
/ — Home page with soft and elegant design, includes a dolphin illustration

/about — Brief description of the project and purpose

/contact — Contact form with a styled submit button

🧩 Issues Encountered & Solutions
SSH Connection Refused
Issue: Unable to connect from host using SCP.
Solution: Enabled SSH with:

bash
Copy
Edit
sudo systemctl enable --now ssh
Flask App Not Accessible from Host
Issue: Port 5000 was blocked.
Solution: Allowed port using:

bash
Copy
Edit
sudo ufw allow 5000
SCP File Transfer Failing
Issue: File not found during scp operation.
Solution: Ensured correct file path, created .zip with:

bash
Copy
Edit
zip -r flask_webapp.zip . 
IP Address Confusion
Issue: Accessing via 127.0.0.1 didn’t work from host.
Solution: Used ip a or hostname -I inside VM to get the bridged adapter IP (192.168.x.x).
