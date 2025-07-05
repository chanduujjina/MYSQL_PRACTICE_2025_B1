# ✅ How to Install MySQL on Windows

This guide will help you install MySQL on a Windows system using the official MySQL Installer.

---

## 🔽 Step 1: Download MySQL Installer

- Go to: [https://dev.mysql.com/downloads/installer/](https://dev.mysql.com/downloads/installer/)
- Choose:
  - **MySQL Installer (Web Installer)** – smaller download, downloads components during install
  - **MySQL Installer (Full Installer)** – includes all components (~400MB)

Click **Download**, then **No thanks, just start my download** if asked to sign up.

---

## 💾 Step 2: Run the Installer

- Double-click the downloaded `.msi` file.
- Choose **Setup Type**:
  - **Developer Default** – installs MySQL Server, Workbench, Shell, and other tools
  - **Server only** – installs just the MySQL Server
  - **Custom** – pick and choose components

✅ Recommended: **Developer Default**

---

## ⚙️ Step 3: Install MySQL Server

- Click **Next** and the installer will check requirements.
- If any dependencies are missing (e.g., Visual C++), the installer will guide you.

Click **Execute** to install components.

---

## 🔐 Step 4: Configure MySQL Server

- Select MySQL version (usually latest 8.x)
- Choose Config Type:
  - **Standalone MySQL Server / Classic MySQL**
- Set Connectivity:
  - Port: `3306` (default)
- Authentication Method:
  - **Use Strong Password Encryption** (recommended)

### 👤 Root Account:
- Set the root password.
- You can also add additional user accounts.

---

## ▶️ Step 5: Start MySQL Server

- MySQL will be added as a **Windows service**.
- You can start/stop it from:
  - **MySQL Workbench**
  - **Services Panel**
  - **Command Line**

---

## 🛠️ Step 6: Test Connection

- Launch **MySQL Workbench**.
- Create a new connection with:
  - Hostname: `localhost`
  - Port: `3306`
  - Username: `root`
  - Password: (set during install)

Click **Test Connection**. ✅

---

## ✅ Done!

You have successfully installed MySQL on your Windows machine.

---

## 📎 Bonus: Open MySQL Shell (Command Line)

To use the MySQL CLI:

```bash
mysql -u root -p
