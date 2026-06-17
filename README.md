# MyAWSApp — Demo Login App 🚀

A simple demo login/signup application built with pure HTML, CSS, and JavaScript.
No backend or database required — perfect for deploying on AWS!

## 🌐 Live Demo Features
- Sign In / Sign Up form
- Demo user pre-loaded: `demo@example.com` / `demo123`
- Mini dashboard shown after login
- Sign out button
- Works 100% in browser — no server needed

## 📁 Files
```
my-demo-app/
├── index.html    ← entire app (1 file only!)
└── README.md
```

## ☁️ Deploy on AWS S3 (Easiest — Free Tier)
1. Go to [AWS S3 Console](https://s3.console.aws.amazon.com)
2. Click **Create bucket** → give it a name
3. Under **Properties** → enable **Static website hosting**
4. Under **Permissions** → uncheck "Block public access"
5. Upload `index.html`
6. Visit the **Bucket website endpoint URL** → your app is live! ✅

## 🖥️ Deploy on AWS EC2 (Ubuntu)
```bash
# SSH into your EC2 instance
ssh -i your-key.pem ubuntu@YOUR_EC2_IP

# Install Apache web server
sudo apt update
sudo apt install -y apache2

# Upload your file
sudo nano /var/www/html/index.html
# (paste the content of index.html and save)

# Visit: http://YOUR_EC2_IP
```

## 🐙 Push to GitHub
```bash
git init
git add .
git commit -m "first commit - demo login app"
git remote add origin https://github.com/YOUR_USERNAME/my-demo-app.git
git branch -M main
git push -u origin main
```

## 🔑 Demo Login
| Email | Password |
|-------|----------|
| demo@example.com | demo123 |

---
Built for AWS deployment demo purposes.
