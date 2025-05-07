# internet_kill_switch
# 🌐 Internet Blocker (Parental Control)

A simple GUI and API-based tool that enables parents to easily disable or re-enable internet access on their child's computer either locally or remotely.

## 📌 Key Features

* Simple GUI for enabling/disabling internet access
* Flask API for remote internet control
* Support for macOS and Windows

---

## 💻 Supported Operating Systems

* **macOS** (Monterey or later recommended)
* **Windows** (Windows 10 or later recommended)

---

## 🔧 Installation

### Common Installation Steps

```bash
git clone https://github.com/yourusername/internet-blocker.git
cd internet-blocker
pip3 install flask tkinter
```

### macOS-specific

No additional installations required (uses built-in macOS commands)

### Windows-specific

Must be run with Administrator privileges.

---

## 🚀 Usage

### Local Usage

```bash
python3 internet_blocker.py
```

Use the GUI to enter the password and enable or disable internet access.

### Remote API Usage

The Flask API runs on the default port `8999`.

* Disable internet:

```bash
curl -X POST "http://<IP>:8999/disable?key=<parent_password>"
```

* Enable internet:

```bash
curl -X POST "http://<IP>:8999/enable?key=<parent_password>"
```

---

## ⚠️ Important Notes

* On **Windows**, always run the script as an Administrator.
* When using the remote API, ensure the parent password is strong and secure.

---

## 📖 Editing Configuration with nano

To edit settings or code directly:

```bash
nano internet_blocker.py
```

To save changes, press `Ctrl+O` followed by `Enter`. To exit, press `Ctrl+X`.

---

## 📄 License
