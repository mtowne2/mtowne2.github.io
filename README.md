<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">home.</a></li>
                <li><a href="#about">about.</a></li>
                <li><a href="#gallery">gallery.</a></li>
            </ul>
        </nav>
        <hr>
    </header>
    <main>
        <section class="intro">
            <h2>Pick A Card, <br> Any Card.</h2>
            <div class="cards">
                <a href="#home" class="card card-home"></a>
                <a href="#about" class="card card-about"></a>
                <a href="#gallery" class="card card-gallery"></a>
            </div>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 My Website</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
@font-face {
    font-family: 'Avenir Black';
    src: url('path/to/avenir-black.woff2') format('woff2'),
         url('path/to/avenir-black.woff') format('woff');
    font-weight: bold;
    font-style: normal;
}

body {
    font-family: 'Avenir Black', Arial, sans-serif;
    background-color: black;
    color: white;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

header {
    text-align: center;
    padding: 20px 0;
}

nav ul {
    list-style: none;
    padding: 0;
    display: flex;
    justify-content: center;
    margin: 0;
}

nav ul li {
    margin: 0 150px; /* Increased spacing 3x more */
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1.2em;
    text-transform: lowercase;
}

hr {
    border: 0;
    height: 2px;
    background-color: white;
    margin-top: 10px;
}

main {
    padding: 20px;
}

.intro h2 {
    font-size: 5em; /* Make the text 5 times larger */
    margin: 20px 0;
    text-align: left;
    padding-left: 50px; /* Move the text to the right */
    opacity: 0;
    transform: translateX(-100px);
    animation: fadeInSlideIn 2s forwards; /* Animation to fade in and slide in */
}

@keyframes fadeInSlideIn {
    0% {
        opacity: 0;
        transform: translateX(-100px);
    }
    100% {
        opacity: 1;
        transform: translateX(0);
    }
}

.cards {
    display: flex;
    justify-content: center;
    gap: 50px;
}

.card {
    width: 300px; /* 3x bigger */
    height: 450px; /* 3x bigger */
    border: 2px solid white;
    border-radius: 10px;
    position: relative;
    transition: transform 0.3s;
    display: flex;
    align-items: center;
    justify-content: center;
    color: black;
    font-size: 3em;
    font-weight: bold;
    text-decoration: none;
}

.card-home {
    background-color: #ff6f61; /* Complementary color */
    transform: rotate(-10deg);
}

.card-about {
    background-color: #6b5b95; /* Complementary color */
    transform: rotate(0deg);
}

.card-gallery {
    background-color: #88b04b; /* Complementary color */
    transform: rotate(10deg);
}

.card:hover {
    transform: scale(1.1);
}

footer {
    text-align: center;
    padding: 5px 0; /* Reduced padding */
    font-size: 0.8em; /* Smaller font size */
    position: fixed;
    bottom: 0;
    width: 100%;
}
document.addEventListener('DOMContentLoaded', function() {
    console.log('JavaScript is working!');
});
