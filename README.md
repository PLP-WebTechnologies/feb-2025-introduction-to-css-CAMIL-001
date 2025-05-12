# Introduction to CSS

## Objectives
Link an external CSS file to an HTML document.
Apply basic styling using selectors.
Use colors, fonts, and spacing effectively.

## Instructions

Create a style.css file.
Apply CSS to a HTML page.
Style elements using:
Classes and IDs.
Color and typography.
Margins, paddings, and borders.

>[!NOTE]
>  - Include at least:
>  - Use of 3 selectors
>  - Style an image
>  - Margin, Padding & Borders
>  - Different font

# Tasks
 - Link an external CSS file.
 - Apply at least 3 different selectors.
 - Improve readability and aesthetics.

Happy Coding! 💻✨

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Website</title>
    <style>
        /* Basic styling for better presentation */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #f2f2f2;
        }
        form {
            margin-top: 20px;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <!-- Ordered list with roman numerals -->
    <h2>Steps to Success:</h2>
    <ol type="I">
        <li>Planning</li>
        <li>Execution</li>
        <li>Evaluation</li>
        <li>Improvement</li>
    </ol>

    <!-- External image from pexels.com -->
    <h2>Featured Image:</h2>
    <img src="https://images.pexels.com/photos/461198/pexels-photo-461198.jpeg" alt="Delicious food" width="500">
    <p><em>Source: Pexels.com</em></p>

    <!-- Contacts table -->
    <h2>Contact List:</h2>
    <table>
        <thead>
            <tr>
                <th>Name</th>
                <th>Address</th>
                <th>Mobile</th>
                <th>Email</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>John Doe</td>
                <td>123 Main St, Nairobi</td>
                <td>0712345678</td>
                <td>john@example.com</td>
            </tr>
            <tr>
                <td>Jane Smith</td>
                <td>456 Park Ave, Mombasa</td>
                <td>0723456789</td>
                <td>jane@example.com</td>
            </tr>
            <tr>
                <td>Mike Johnson</td>
                <td>789 Hill Rd, Kisumu</td>
                <td>0734567890</td>
                <td>mike@example.com</td>
            </tr>
            <tr>
                <td>Sarah Williams</td>
                <td>321 Valley Dr, Nakuru</td>
                <td>0745678901</td>
                <td>sarah@example.com</td>
            </tr>
            <tr>
                <td>David Brown</td>
                <td>654 Lake View, Eldoret</td>
                <td>0756789012</td>
                <td>david@example.com</td>
            </tr>
        </tbody>
    </table>

    <!-- Registration form -->
    <h2>Registration Form</h2>
    <form id="registrationForm">
        <!-- Name field -->
        <div class="form-group">
            <label for="name">Full Name:</label>
            <input type="text" id="name" name="name" placeholder="Enter your full name" required>
        </div>

        <!-- Email field -->
        <div class="form-group">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Enter your email" required>
        </div>

        <!-- Password field -->
        <div class="form-group">
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" placeholder="Create a password" minlength="8" required>
        </div>

        <!-- Date field -->
        <div class="form-group">
            <label for="dob">Date of Birth:</label>
            <input type="date" id="dob" name="dob" required>
        </div>

        <!-- Dropdown menu -->
        <div class="form-group">
            <label for="country">Country:</label>
            <select id="country" name="country" required>
                <option value="">Select your country</option>
                <option value="kenya">Kenya</option>
                <option value="uganda">Uganda</option>
                <option value="tanzania">Tanzania</option>
                <option value="rwanda">Rwanda</option>
                <option value="other">Other</option>
            </select>
        </div>

        <!-- Radio buttons -->
        <div class="form-group">
            <label>Gender:</label>
            <div>
                <input type="radio" id="male" name="gender" value="male" required>
                <label for="male">Male</label>
            </div>
            <div>
                <input type="radio" id="female" name="gender" value="female">
                <label for="female">Female</label>
            </div>
            <div>
                <input type="radio" id="other" name="gender" value="other">
                <label for="other">Other</label>
            </div>
        </div>

        <!-- Checkboxes -->
        <div class="form-group">
            <label>Interests:</label>
            <div>
                <input type="checkbox" id="sports" name="interests" value="sports">
                <label for="sports">Sports</label>
            </div>
            <div>
                <input type="checkbox" id="music" name="interests" value="music">
                <label for="music">Music</label>
            </div>
            <div>
                <input type="checkbox" id="reading" name="interests" value="reading">
                <label for="reading">Reading</label>
            </div>
        </div>

        <!-- Submit button -->
        <button type="submit">Register</button>
    </form>

    <!-- Simple form validation script -->
    <script>
        document.getElementById('registrationForm').addEventListener('submit', function(event) {
            if (!this.checkValidity()) {
                event.preventDefault();
                alert('Please fill in all required fields correctly.');
            }
        });
    </script>
</body>
</html>

 OR 
 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Web Page</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&family=Open+Sans&family=Playfair+Display:wght@700&family=Roboto&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="main-container">
        <header class="page-header">
            <h1>Welcome to Our Website</h1>
            <p>Discover our amazing services</p>
        </header>

        <div id="special-offer">
            <p>✨ Special limited-time offer! Sign up today for 20% off. ✨</p>
        </div>

        <img src="https://images.pexels.com/photos/3184418/pexels-photo-3184418.jpeg" alt="Team working together" class="featured-image">

        <div class="card">
            <h2>Our Services</h2>
            <p>We offer a wide range of professional services to help your business grow.</p>
            <a href="#" class="btn">Learn More</a>
        </div>

        <div class="card">
            <h2>Contact Us</h2>
            <p>Reach out to our team for more information about what we can do for you.</p>
            <a href="#" class="btn">Contact Now</a>
        </div>
    </div>
</body>
</html>
