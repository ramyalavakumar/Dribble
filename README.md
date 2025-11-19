# Project Responsive Web Design using Bootstrap
## Date:13.10.2025

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
dribble.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" crossorigin="anonymous">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8f7f4;
        }
        .navbar-brand.dribbble-pink {
            color: #4C85EA;
        }
        .dribbble-pink-btn {
            background-color: #4C85EA;
            color: white;
            border-radius: 6px;
            font-weight: 600;
            padding: 6px 12px;
            transition: background-color 0.2s;
        }
        .dribbble-pink-btn:hover {
            background-color: #3B7AE2;
        }
        .hero-heading {
            font-size: 2.5rem;
            font-weight: 800;
            margin-top: 3rem;
            margin-bottom: 2rem;
        }
        .shot-placeholder {
            height: 200px;
            background-color: #ffffff;
            border: 1px solid #ddd;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        }
        .shot-placeholder img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .search-bar-container input {
            border-radius: 30px;
            padding: 0.75rem 1.5rem;
        }
    </style>
</head>
<body>

<nav class="navbar bg-white shadow-sm">
    <div class="container d-flex justify-content-between align-items-center py-2">
        <a class="navbar-brand dribbble-pink" href="#" style="font-weight: 800;">dribbble</a>

        <div class="d-flex align-items-center gap-3">
            <a class="text-decoration-none text-dark" href="#">Sign In</a>
            <a class="btn dribbble-pink-btn" href="#">Sign Up</a>
        </div>
    </div>
</nav>

<section class="container text-center py-5">
    <h1 class="hero-heading">
        The world’s leading community for creatives
    </h1>
    <p class="lead text-muted mb-4">
        Design inspiration, work, and learning—simplified.
    </p>

    <div class="search-bar-container mx-auto" style="max-width: 450px;">
        <input type="search" class="form-control" placeholder="Search for shots...">
    </div>
</section>

<main class="container mb-5 mt-4">
    <h2 class="h5 mb-4 text-dark">Trending Designs</h2>
    <div class="row g-4" id="shot-grid">
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">User Name</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Design Studio</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Freelancer</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Animator</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Web Coder</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Icon Artist</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Design Pro</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Creative Hub</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Sketcher</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Vector Art</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Pixel Power</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">UI Ninja</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">App Creator</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Brand Builder</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Illustrator</small>
        </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 shot-item">
            <div class="shot-placeholder"></div>
            <small class="text-muted mt-2 d-block shot-user-name">Icon Artist</small>
        </div>
    </div>
</main>

<footer class="bg-white py-3 border-top">
    <div class="container text-center">
        <p class="text-muted mb-0" style="font-size: 0.85rem;">© 2025 Clone. Basic Design.</p>
    </div>
</footer>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" crossorigin="anonymous"></script>

<script>
    document.addEventListener('DOMContentLoaded', () => {
        const shotItems = document.querySelectorAll('.shot-item');
        
        const names = [
            "Alexia G.", "Design Flow", "Studio Z", "Pixel Guru", 
            "Creative Cat", "Jake M.", "Motion Co.", "UX Master",
            "Art King", "Vector Guy", "Digital Dreamer", "Code Artist",
            "Design Pro", "Creative Hub", "Sketcher", "Vector Art",
            "Pixel Power", "UI Ninja", "App Creator", "Brand Builder",
            "Illustrator"
        ];
        
        const getRandom = (arr) => arr[Math.floor(Math.random() * arr.length)];
        
        let imageIdCounter = 100;

        shotItems.forEach((item, index) => {
            const placeholder = item.querySelector('.shot-placeholder');
            const userNameElement = item.querySelector('.shot-user-name');
            
            let imageId;
            let randomName;

            if (index === shotItems.length - 1) {
                imageId = 250; 
                randomName = "Featured Artist"; 
            } else {
                imageId = imageIdCounter;
                imageIdCounter++;
                randomName = getRandom(names);
            }
            
            userNameElement.textContent = randomName;

            const imageUrl = `https://picsum.photos/id/${imageId}/400/300`;
            
            const img = document.createElement('img');
            img.src = imageUrl;
            img.alt = `Design Shot by ${randomName}`;
            
            placeholder.innerHTML = ''; 
            placeholder.appendChild(img);
        });
    });
</script>

</body>
</html>


## OUTPUT:
<img width="1029" height="481" alt="Screenshot 2025-10-13 174449" src="https://github.com/user-attachments/assets/83f3fd6c-fa70-46d4-8f27-778460183fae" />

<img width="1034" height="439" alt="Screenshot 2025-10-13 174512" src="https://github.com/user-attachments/assets/a302647f-5945-4a69-9d1e-5a0e7e4b3ce4" />


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully. 
