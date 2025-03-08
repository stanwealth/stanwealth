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
<!DOCTYPE html>
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
            background:(135 deg, #2c3e50, #34495e);
            color: #fff;
            padding: 40 px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background: #1abc9c;
            padding: 15 px;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            padding: 15 px 25 px;
            font-weight: bold;
            transition: background 0.3 s ease;
        }
        nav a:hover {
            background: #16a085;
            border-radius: 5 px;
        }
        .banner {
            background: url('https://source.unsplash.com/1600x600/?finance,wealth') no-repeat center;
            background-size: cover;
            height: 300 px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 30 px;
            font-weight: bold;
            text-shadow: 2 px 2 px 8 px rgba (0, 0, 0, 0.5);
        }
        .container {
            max-width: 1000 px;
            margin: 30 px auto;
            padding: 20 px;
            background: white;
            box-shadow: 0 0 15 px rgba (0, 0, 0, 0.2);
            border-radius: 10 px;
        }
        .services {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        .service-card {
            background: #ecf0f1;
            padding: 20 px;
            margin: 10 px;
            flex: 1 1 45 %;
            border-radius: 8 px;
            box-shadow: 0 4 px 8 px rgba (0, 0, 0, 0.1);
        }
        footer {
            text-align: center;
            padding: 20 px;
            background: #2c3e50;
            color: white;
            margin-top: 20 px;
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
    <div class="banner">
        Building Wealth for a Better Future
    </div>
    <div class="container">
        <h2 id="home">Welcome to Stan Wealth</h2>
        <p>At Stan Wealth, we provide expert financial planning and wealth management services to help you achieve your financial goals.</p>
        <h2 id="services">Our Services</h2>
        <div class="services">
            <div class="service-card">
                <h3>Investment Management</h3>
                <p>Smart strategies to grow and secure your wealth.</p>
            </div>
            <div class="service-card">
                <h3>Retirement Planning</h3>
                <p>Ensuring a stable and fulfilling future for you.</p>
            </div>
            <div class="service-card">
                <h3>Tax Optimization</h3>
                <p>Maximizing your earnings with strategic tax planning.</p>
            </div>
            <div class="service-card">
                <h3>Estate Planning</h3>
                <p>Preserving your legacy for generations to come.</p>
            </div>
        </div>
        <h2 id="about">About Us</h2>
        <p>Stan Wealth has been a leader in financial services for over a decade, guiding clients towards financial success with expert advice and personalized strategies.</p>
        <h2 id="contact">Contact Us</h2>
        <p>Email: contact@stanwealth.com</p>
        <p>Phone: (123) 456-7890</p>
        <p>Address: 123 Wealth Street, Finance City, USA</p>
    </div>
    <footer>
        <p>&copy; 2025 Stan Wealth. All rights reserved.</p>
    </footer>
</body>
</html>
