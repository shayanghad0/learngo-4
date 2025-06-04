# 🔐 Go CLI Auth System
A simple user management system in Go. Supports user registration, login, and dashboard (edit profile). Stores data in a JSON file. All from the terminal.

- 🧱 Beginner → Intermediate | 📦 JSON-based storage | 💡 Learn Go with real practice

## 📦 Features

- 👤 Register (username, password, email, name, age)

- 🔑 Login with password verification (hashed)

- 🧾 Dashboard: edit all profile fields

- 💾 JSON file acts as a mini database

- ✨ Fully terminal-based, beginner-friendly

## 📁 Project Structure>
```
.
├── main.go         # main logic
└── users.json      # local JSON database (auto-created)
```

## 🚀 Getting Started
1. Clone the repo
```
git clone https://github.com/yourusername/go-auth-cli.git
cd go-auth-cli
```
2. Run it
```
go run main.go
```
🧪 Sample Workflow
```
--- MENU ---
1. Register
2. Login
3. Exit
Choose: 1

Username: shayan
Password: ****
Email: shayan@mail.com
Full Name: Shayan Dev
Age: 23

✅ Registration complete.

--- MENU ---
Choose: 2

Username: shayan
Password: ****

✅ Logged in as shayan

--- DASHBOARD ---
1. Edit Username
2. Edit Password
3. Edit Email
4. Edit Name
5. Edit Age
6. Logout
```
## 🔐 Password Security
- Passwords are stored securely using SHA-256 hashing:
> hash := sha256.Sum256([]byte(password))
## 📁 JSON Database Example
```
{
  "shayan": {
    "username": "shayan",
    "password": "1c472af2d3...", 
    "email": "shayan@mail.com",
    "name": "Shayan Dev",
    "age": 23
  }
}
```
## 🧠 Learning Goals
- Structs & JSON marshalling

- File read/write with os and encoding/json

- Input handling with fmt.Scan & bufio.Reader

- Basic security concepts (hashing)

- Loop logic and CLI UX in Go


## 🧠 Part of...
>📘 die <= learn Go => master

## 📜 License
> MIT — free to use, learn, remix.