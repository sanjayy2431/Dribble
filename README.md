# Project Responsive Web Design using Bootstrap
## Date: 14/11/2024

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble Clone</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: 'Pacifico', cursive;
            margin: 0;
            padding: 0;
            background-image: url('your-image-url.jpg'); /* Add your image URL here */
            background-size: cover; /* Ensure the image covers the entire background */
            background-position: center; /* Position the image in the center */
            background-repeat: no-repeat; /* Prevent the image from repeating */
            color: #2c3e50; /* Dark, contrasting text */
        }
        .gallery-item {
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease;
        }
        .gallery-item:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }
        .gallery-img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
    </style>
    <!-- Google Font for Pacifico -->
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <a class="navbar-brand" href="#">Dribbble</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item"><a class="nav-link" href="#">Shots</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Designers</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Teams</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Community</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Jobs</a></li>
                <li class="nav-item"><a class="btn btn-primary" href="#">Sign Up</a></li>
            </ul>
        </div>
    </nav>

    <!-- Main Content Section -->
    <div class="container mt-4">
        <div class="text-center mb-4 header-section">
            <h3>What are you working on?</h3>
            <p class="lead">Dribbble is show and tell for designers.</p>
        </div>

        <!-- Gallery Section -->
        <div class="row gallery-section">
            <!-- Gallery Items (8 items in total) -->
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="one.jpg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">DENIM</p>
                        <small class="text-muted">Levis</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="two.jpg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">SNEAKERS</p>
                        <small class="text-muted">PUMA</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="three.jpg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">SHOES</p>
                        <small class="text-muted">WOODLAND</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="four.jpg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">HEELS</p>
                        <small class="text-muted">ZARA</small>
                    </div>
                </div>
            </div>
            <!-- Additional Gallery Items -->
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="five.jpg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">WATCH</p>
                        <small class="text-muted">SWATCH</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="six.jpg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">SNEAKERS</p>
                        <small class="text-muted">NIKE</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="seven.jpg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">HEELS</p>
                        <small class="text-muted">MACYS</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="eig.jpg" class="card-img-top gallery-img" alt="Design Thumbnail">
                    <div class="card-body text-center">
                        <p class="card-title">PERFUMES</p>
                        <small class="text-muted">corno de ouro</small>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="bg-dark text-white text-center py-3">
        <p>© Dribbble. All rights reserved.</p>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

```
css

@import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');

body {
    font-family: 'Pacifico', cursive;
    margin: 0;
    padding: 0;
    background-color: #bcd4d4; /* Soft teal background */
    color: #2c3e50; /* Dark, contrasting text */
}

/* Navbar Customization */
.navbar {
    background-color: #00695c; /* Dark teal background */
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1); /* Slight shadow */
}

.navbar-brand, .navbar-nav .nav-link {
    color: #ffffff !important;
}

.navbar-nav {
    flex-direction: row;
}

.navbar-nav .nav-link {
    padding: 0 15px;
}

.nav-item .btn-primary {
    background-color: #ff7043; /* Coral for buttons */
    border-color: #ff7043;
}

.nav-item .btn-primary:hover {
    background-color: #d84315; /* Darker coral on hover */
    border-color: #d84315;
}

/* Header Section */
.header-section h3 {
    font-weight: bold;
    color: #00695c; /* Dark teal */
}

.header-section p {
    font-size: 1.2em;
    color: #37474f; /* Darker, readable text */
}

/* Gallery and Card adjustments */
.gallery-container {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 20px;
    padding: 20px;
}

/* Card Styling */
.card {
    background-color: #ffffff;
    border: 1px solid #cfd8dc;
    border-radius: 10px;
    box-shadow: 0px 6px 12px rgba(0, 0, 0, 0.08); /* Light shadow */
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 0; /* No padding around card */
    margin-bottom: 20px;
}

.card:hover {
    transform: translateY(-5px); /* Lift effect */
    box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.15); /* Stronger shadow on hover */
}

/* Adjusted Card Image Styling */
.gallery-img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 10px 10px 0 0; /* Rounded top corners only */
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    margin-bottom: 0; /* No bottom margin */
}

.card:hover .gallery-img {
    transform: scale(1.05); /* Zoom effect on hover */
    box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.25); /* Subtle shadow on hover */
}

/* Card Content */
.card-title {
    font-weight: bold;
    font-size: 1.1rem;
    color: #00695c; /* Dark teal for titles */
    text-align: center;
    margin-top: 15px;
}

.card-body {
    padding: 20px;
    text-align: center;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

/* Footer */
footer {
    background-color: #00695c;
    color: #ffffff;
    text-align: center;
    padding: 25px;
    font-size: 0.9em;
    margin-top: 40px;
    box-shadow: 0px -2px 5px rgba(0, 0, 0, 0.1); /* Shadow above footer */
}

/* Responsive Design */
@media (max-width: 768px) {
    .navbar-nav {
        flex-direction: column;
        text-align: center;
        padding: 10px 0;
    }

    .gallery-section {
        margin-top: 20px;
    }

    .card-body {
        padding: 10px;
    }
}

@media (max-width: 480px) {
    .header-section h3 {
        font-size: 1.5em;
    }

    .header-section p {
        font-size: 1em;
    }
}
```

## OUTPUT:
![Screenshot 2024-11-13 115635](https://github.com/user-attachments/assets/0f70d60d-ae31-42ac-8fa7-86a044548d12)


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
