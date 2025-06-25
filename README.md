# 🛡️ Django reCAPTCHA v2 Integration Guide

![Django reCAPTCHA Demo](https://example.com/recaptcha-demo.gif) *Example of reCAPTCHA in action*

## 🌟 Why Use reCAPTCHA?
| Problem | Solution |
|---------|----------|
| Spam submissions | ✅ Blocks 99% of bots |
| Fake accounts | ✅ Human verification |
| Brute force attacks | ✅ Rate limiting |

## 🚀 Quick Start

### 1. Django Configuration / settings.py

INSTALLED_APPS = [
    ...,
    'captcha',  # Must be added
]

# Get keys from https://www.google.com/recaptcha/admin
RECAPTCHA_PUBLIC_KEY = '6Lc...'  # Frontend key
RECAPTCHA_PRIVATE_KEY = '6Ld...'  # Backend key (keep secret!)


### 2. Environment Setup
```bash
# Create and activate virtual environment
python -m venv venv
# Linux/Mac:
source venv/bin/activate
# Windows:
.\venv\Scripts\activate

# Install packages
pip install django django-recaptcha