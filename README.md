# bia-website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BIA at USC</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }
        header {
            background-color: #0073e6;
            color: white;
            text-align: center;
            padding: 20px;
        }
        nav {
            text-align: center;
            margin: 20px 0;
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #0073e6;
        }
        .container {
            width: 80%;
            margin: auto;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1, h2 {
            color: #333;
        }
        footer {
            text-align: center;
            background-color: #0073e6;
            color: white;
            padding: 10px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to BIA at USC</h1>
        <p>Your bridge to international and American cultures</p>
    </header>

    <nav>
        <a href="#about">About Us</a>
        <a href="#events">Events</a>
        <a href="#membership">Membership</a>
        <a href="#sponsors">Sponsors</a>
        <a href="#contact">Contact</a>
    </nav>

    <div class="container" id="about">
        <h2>About BIA at USC</h2>
        <p>BIA at USC is a student organization that was founded in March 2024 with the goal to create a vibrant international student community and serve as a bridge between international students and American cultures.</p>
    </div>

    <div class="container" id="events">
        <h2>Upcoming Events</h2>
        <ul>
            <li>Welcome Party - Fall 2024</li>
            <li>Halloween Party - October 2024</li>
            <li>Spring/Fall Formal - 2025</li>
        </ul>
    </div>

    <footer>
        <p>&copy; 2024 BIA at USC - All Rights Reserved</p>
    </footer>
</body>
</html>

<style>
    /* Enhanced Navbar */
    nav {
        background-color: #0073e6;
        position: sticky;
        top: 0;
        width: 100%;
        z-index: 1000;
    }

    .navbar {
        list-style: none;
        padding: 0;
        margin: 0;
        display: flex;
        justify-content: center;
        gap: 15px;
    }

    .navbar li {
        display: inline;
    }

    .navbar a {
        color: white;
        text-decoration: none;
        padding: 15px 20px;
        display: inline-block;
        transition: background-color 0.3s;
    }

    .navbar a:hover {
        background-color: #005bb5;
    }
</style>

<div class="container" id="membership">
    <h2>Join BIA at USC</h2>
    <form id="membershipForm">
        <label for="name">Name:</label><br>
        <input type="text" id="name" name="name" required><br><br>
        <label for="email">Email:</label><br>
        <input type="email" id="email" name="email" required><br><br>
        <label for="studentID">USC Student ID:</label><br>
        <input type="text" id="studentID" name="studentID" required><br><br>
        <input type="submit" value="Join Now">
    </form>
    <p id="formMessage"></p>
</div>

<script>
    // Simple form validation
    document.getElementById('membershipForm').addEventListener('submit', function (e) {
        e.preventDefault();
        const name = document.getElementById('name').value;
        const email = document.getElementById('email').value;
        const studentID = document.getElementById('studentID').value;
        
        if (name && email && studentID) {
            document.getElementById('formMessage').textContent = "Thank you for joining BIA at USC!";
        } else {
            document.getElementById('formMessage').textContent = "Please fill out all fields.";
        }
    });
</script>

<style>
    /* Membership Form Styles */
    input[type="text"], input[type="email"] {
        width: 100%;
        padding: 10px;
        margin: 5px 0 10px 0;
        box-sizing: border-box;
    }

    input[type="submit"] {
        background-color: #0073e6;
        color: white;
        padding: 10px 20px;
        border: none;
        cursor: pointer;
    }

    input[type="submit"]:hover {
        background-color: #005bb5;
    }

    #formMessage {
        color: green;
        font-weight: bold;
        margin-top: 10px;
    }
</style>
<div class="container" id="contact">
    <h2>Contact Us</h2>
    <p>If you have any questions, feel free to reach out!</p>
    <form id="contactForm">
        <label for="contactName">Name:</label><br>
        <input type="text" id="contactName" name="contactName" required><br><br>
        <label for="contactEmail">Email:</label><br>
        <input type="email" id="contactEmail" name="contactEmail" required><br><br>
        <label for="message">Message:</label><br>
        <textarea id="message" name="message" rows="4" required></textarea><br><br>
        <input type="submit" value="Send Message">
    </form>
    <p id="contactMessage"></p>
</div>

<script>
    // Simple contact form handler
    document.getElementById('contactForm').addEventListener('submit', function (e) {
        e.preventDefault();
        const contactName = document.getElementById('contactName').value;
        const contactEmail = document.getElementById('contactEmail').value;
        const message = document.getElementById('message').value;
        
        if (contactName && contactEmail && message) {
            document.getElementById('contactMessage').textContent = "Your message has been sent!";
        } else {
            document.getElementById('contactMessage').textContent = "Please fill out all fields.";
        }
    });
</script>

<style>
    /* Contact Form Styles */
    textarea {
        width: 100%;
        padding: 10px;
        margin: 5px 0 10px 0;
        box-sizing: border-box;
    }

    #contactMessage {
        color: green;
        font-weight: bold;
        margin-top: 10px;
    }
</style>
/* Fade-in Animation */
@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

/* Apply the animation to sections */
.container {
    animation: fadeIn 1.5s ease-in;
}

/* Button Hover Effects */
input[type="submit"] {
    transition: background-color 0.3s, transform 0.3s;
}

input[type="submit"]:hover {
    background-color: #005bb5;
    transform: scale(1.05);
}
/* Mobile-first design */
body {
    margin: 0;
    font-family: Arial, sans-serif;
}

.container {
    padding: 20px;
}

/* Media Queries for Tablets and Desktops */
@media (min-width: 600px) {
    .container {
        width: 80%;
        margin: auto;
    }
}

@media (min-width: 900px) {
    .navbar {
        justify-content: flex-start;
        gap: 25px;
    }
}

<footer>
    <p>&copy; 2024 BIA at USC - All Rights Reserved</p>
    <p>Follow us on: 
        <a href="#">WeChat</a> | 
        <a href="#">Xiaohongshu</a>
    </p>
    <p>Contact: <a href="mailto:contact@biaatusc.com">contact@biaatusc.com</a></p>
</footer>

<style>
    footer {
        text-align: center;
        background-color: #0073e6;
        color: white;
        padding: 20px;
        position: relative;
        bottom: 0;
        width: 100%;
    }

    footer a {
        color: white;
        text-decoration: underline;
    }

    footer a:hover {
        color: #ffcc00;
    }
</style>
