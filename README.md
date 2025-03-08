## Hi there 👋

import zipfile
import os

# Define file structure
file_name = "stan_wealth.html"
zip_name = "/mnt/data/stan_wealth_website.zip"
html_content = """<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stan Wealth - Wealth Management</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }
        body {
            background: #f4f4f4;
            color: #333;
        }
        header {
            background: #2c3e50;
            color: #fff;
            padding: 15;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background: #34495e;
            padding: 10;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            padding: 1020;
        }
        nav a:hover {
            background: #2c3e50;
        }
        .container {
            max-width: 1000;
            margin: 20 auto;
            padding: 20;
            background: #fff;
            box-shadow: 0 0 10 (0, 0, 0, 0.1);
            border-radius: 5;
        }
        footer {
            text-align: center;
            padding: 15;
            background: #2c3e50;
            color: white;
            position: relative;
            bottom: 0;
            width: 100;
        }
    </style>
</head>
<body>
    <header>
        <h1>Stan Wealth</h1>
        <p>Your Trusted Wealth Management Partner</p>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#services">Services</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>
    <div class="container">
        <h2 id="home">Home</h2>
        <p>At Stan Wealth, we provide expert financial planning and wealth management services to help you achieve your financial goals.</p>
        <h2 id="services">Our Services</h2>
        <ul>
            <li>Investment Management</li>
            <li>Retirement Planning</li>
            <li>Tax Optimization</li>
            <li>Estate Planning</li>
        </ul>
        <h2 id="about">About Us</h2>
        <p>Stan Wealth has been a leader in financial services for over a decade, guiding clients towards financial success with expert advice and personalized strategies.</p>
        <h2 id="contact">Contact</h2>
        <p>Email: contact@stanwealth.com</p>
        <p>Phone: (123) 456-7890</p>
        <p>Address: 123 Wealth Street, Finance City, USA</p>
    </div>
    <footer>
        <p>&copy; 2025 Stan Wealth. All rights reserved.</p>
    </footer>
</body>
</html>"""

# Create a ZIP file
with zipfile.ZipFile(zip_name, 'w') as zipf:
    with open(file_name, 'w', encoding='utf-8') as f:
        f.write(html_content)
    zipf.write(file_name)

# Remove the temporary file
os.remove(file_name)

# Return the ZIP file path
zip_name
