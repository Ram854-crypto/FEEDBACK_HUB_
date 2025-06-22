# FEEDBACK_HUB_

# 🌟 Lightweight Feedback System

A complete, responsive web application designed for managing manager-employee feedback in a lightweight setup. Ideal for demo use, internal team feedback, or performance tracking — all from the comfort of Google Colab.

---

## 🔧 Tech Stack

| Component      | Technology         |
|----------------|--------------------|
| Backend        | Python Flask       |
| Frontend       | HTML, CSS          |
| Database       | SQLite             |
| Tunneling      | Pyngrok / Cloudflare / LocalTunnel / Colab Proxy |
| Hosting        | Google Colab (Jupyter-based server) |

---

## ✨ Features

- 👤 Role-based Authentication (Manager / Employee)
- 📝 Feedback Submission with Sentiment & Tags
- 📊 Dashboards with Team & Feedback Stats
- ✅ Feedback Acknowledgment with Comments
- 🔄 Real-time Form Submission & Editing
- 🎨 Modern and Responsive UI (No React Needed!)
- 🔐 Secure Password Hashing and Session Management

---

## 🚀 Setup Instructions (for Google Colab)

### ✅ Step 1: Install Dependencies

```bash
!pip install flask werkzeug pyngrok



 Step 2: Run the App
You can start the app in one of three ways:

🔹 Option 1 (Recommended): Google Colab Proxy
run_with_colab_proxy()

🔹 Option 2: Auto-Tunnel (tries multiple tunnels)
run_app()


🔹 Option 3: Manual Colab Proxy
Run:
run_app()
Then in a new cell:
from google.colab.output import eval_js
print("🌐 URL:", eval_js('google.colab.kernel.proxyPort(5000)'))






🧪 Demo Accounts

| Role     | Username       | Password     |
| -------- | -------------- | ------------ |
| Manager  | `john_manager` | `manager123` |
| Employee | `alice_emp`    | `emp123`     |
| Employee | `bob_emp`      | `emp123`     |






 Security Highlights
1. Password hashing (werkzeug.security)

2. Role-based access control

3. SQL injection resistance via parameterized queries

4. Secure session handling



📱 Design Highlights
1. Clean dashboard with performance metrics

2. Fully responsive layout (mobile-friendly)

3. Gradient-based UI with animated cards

4. Modal forms for feedback & acknowledgment

5. Dashboard separation for managers and employees




🛠️ Development Notes
1. Single-file App: Easy to deploy and understand.

2. No External Templates: Everything is embedded via render_template_string.

3. SQLite for Local/Colab Use: Zero setup required.

📌 Important Notes
1. The app is primarily designed for use in Google Colab.

2. Works best with run_with_colab_proxy() for automatic setup.

3. You can use ngrok, cloudflared, or localtunnel depending on availability.

📜 License
This project is open-source under the MIT License.


