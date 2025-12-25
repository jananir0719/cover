# Ex.06 Book Front Cover Page Design
## Date:

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Book Cover</title>
  <style>
  body {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    margin: 0;
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
  }
  
  .book-cover {
    width: 300px;
    height: 450px;
    perspective: 1000px; /* Gives a 3D effect on hover */
  }
  
  .book-cover-inner {
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center;
    transition: transform 0.8s;
    transform-style: preserve-3d;
  }
  
  .book-cover:hover .book-cover-inner {
    transform: rotateY(-30deg); /* Slight rotation on hover */
  }
  
  .cover-front {
    position: absolute;
    width: 100%;
    height: 100%;
    -webkit-backface-visibility: hidden; /* Hide the back of the element when rotated */
    backface-visibility: hidden;
    background-color:#a40e7a; /* Dark cover color */
    color: black; /* Light text color */
    border-radius: 8px;
    box-shadow: 10px 10px 20px plum; /* Creates a shadow effect */
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 20px;
  }
  
  .book-title {
    font-size: 2em;
    margin-bottom: 0.5em;
  }
  
  .book-author {
    font-size: 1.2em;
    font-style: italic;
  }
  
  /* Additional styles for responsiveness */
  @media (max-width: 600px) {
    .book-cover {
      width: 250px;
      height: 375px;
    }
    .book-title {
      font-size: 1.8em;
    }
  }
</style>
</head>
<body>

  <div class="book-cover">
    <div class="book-cover-inner">
      <div class="cover-front">
        <h1 class="book-title">FUNDAMENTALS OF WEB</h1>
        <p class="book-author">By Maddy</p>
      </div>
    </div>
  </div>

</body>
</html>



## OUTPUT:
<img width="622" height="727" alt="image" src="https://github.com/user-attachments/assets/d1a92ed4-1169-408c-81b4-b567ddb066a0" />


## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
