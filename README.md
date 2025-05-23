# Ex.08 Design of Interactive Image Gallery
## Date: 12.05.2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>SERIES</h1>
    </header>
    <div class="gallery">
        <div class="gallery-item" onclick="openModal(this)">
            <img src="c:\Users\admin\Downloads\1_URQlzzR5MHI9Lkm63wrduw.jpg" >
        </div>
        <div class="gallery-item" onclick="openModal(this)">
            <img src="c:\Users\admin\Downloads\images.jpeg"  >
        </div>
        <div class="gallery-item" onclick="openModal(this)">
            <img src="c:\Users\admin\Downloads\maxton-hall.webp" >
        </div>
        <div class="gallery-item" onclick="openModal(this)">
            <img src="c:\Users\admin\Downloads\download (1).jpeg" >
        </div>
    </div>

    <div id="modal" class="modal">
        <span class="close" onclick="closeModal()">&times;</span>
        <img class="modal-content" id="modalImage">
        <div id="caption"></div>
    </div>

    <script src="style.js"></script>
</body>
</html>
body{
    background-color:lightslategray ;  
    font-family: Arial, sans-serif;  
    margin: 0; 
    padding: 20px;  
    text-align: center;
    color:cornsilk;
};
img{
    align-content: center;
}
.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 16px;
    padding: 16px;
}

.gallery-item img {
    width: 100%;
    height: auto;
    border-radius: 8px;
    cursor: pointer;
    transition: transform 0.3s ease;
}

.gallery-item img:hover {
    transform: scale(1.1);
}
#modalImage {
    transition: transform 0.5s ease-in-out;
    transform: scale(1); /* Default scale */
}

#modalImage.zoomed {
    transform: scale(1.5); /* Zoomed-in scale */
}
```
## OUTPUT:


![Screenshot (164)](https://github.com/user-attachments/assets/bd4ccae4-13fb-4d95-bc68-0738cbb80d40)


![Screenshot (165)](https://github.com/user-attachments/assets/0675b8d1-7e79-4423-a7ec-59edfa75dc45)


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
