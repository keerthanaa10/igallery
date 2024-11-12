# Ex-7: Interactive Image Gallery
## Date: 12-11-2024

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

### index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1 class="title">Interactive Photo Gallery</h1>
    <div id="image">Hover over an image below to display here.</div>
    
    <div class="gallery">
        <img class = "preview" alt = "pic1" src = "https://images.unsplash.com/photo-1729505621471-ea543f4a0a6b?q=80&w=1887&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" alt = "pic2" src = "https://plus.unsplash.com/premium_photo-1731138873437-abd758179553?q=80&w=1929&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" src = "https://images.unsplash.com/photo-1726384865480-2509fa0857bf?q=80&w=1885&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt = "pic3" onmouseover = "upDate(this)" onmouseout = "unDo()">
        <img class = "preview" alt = "pic4" src = "https://images.unsplash.com/photo-1726499642197-e84767270f24?q=80&w=1884&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" alt = "pic5" src = "https://images.unsplash.com/photo-1731082417879-710ff0c868ae?q=80&w=1887&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" src = "https://images.unsplash.com/photo-1729508895264-d61e3f6587fa?q=80&w=1919&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt = "pic6" onmouseover = "upDate(this)" onmouseout = "unDo()">
    </div>
    <script src="script.js"></script>
</body>
</html>
```

### gallery.css
```css
body{
    margin: 2%;
    border: 1px solid black;
    background-color: #474747;
}
.title{
    text-align: center;
}
#image{
    line-height:650px;
    width: 375px;
    height: 400px;
    border:5px solid black;
    margin:0 auto;
    background-color: #000000;
    background-image: url('');
    background-repeat: no-repeat;
    color:#FFFFFF;
    text-align: center;
    background-size: 100%;
    margin-bottom:25px;
    font-size: 150%;
}
.preview{
    width:10%;
    margin-left:17%;
border: 10px solid black;
}
img{
    width:95%;
}
```

### gallery.js
```js
const imageDiv = document.getElementById('image');
const originalImageUrl = ''; 
const originalText = "Hover over an image below to display here.";

function upDate(previewPic) {
    imageDiv.style.backgroundImage = `url('${previewPic.src}')`;
    
    imageDiv.innerHTML = previewPic.alt;
}

function unDo() {
    imageDiv.style.backgroundImage = `url('${originalImageUrl}')`;
    imageDiv.innerHTML = originalText;
}
```
## WEBSITE URL
```
https://codepen.io/Harish_-Ammu/pen/bGXVBVW
```
## OUTPUT:
![alt text]({2A4CDCD7-4778-4019-B872-92D5313854AE}.png)
![alt text](image.png)
![alt text](image-1.png)

## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
`