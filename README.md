<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MovieFlix</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins', sans-serif;
}

body{
    background:#0f0f0f;
    color:white;
}

/* Navbar */
nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 60px;
    background:rgba(0,0,0,0.9);
    position:sticky;
    top:0;
    z-index:1000;
}

nav h1{
    color:#e50914;
    font-size:28px;
}

nav ul{
    list-style:none;
    display:flex;
    gap:25px;
}

nav ul li{
    cursor:pointer;
    transition:0.3s;
}

nav ul li:hover{
    color:#e50914;
}

/* Hero Section */
.hero{
    height:85vh;
    background:
        linear-gradient(to right, rgba(0,0,0,0.8), rgba(0,0,0,0.3)),
        url('https://images.unsplash.com/photo-1524985069026-dd778a71c7b4') center/cover no-repeat;
    display:flex;
    align-items:center;
    padding-left:60px;
}

.hero-content{
    max-width:500px;
}

.hero-content h2{
    font-size:55px;
    margin-bottom:20px;
}

.hero-content p{
    margin-bottom:25px;
    line-height:1.6;
    color:#ccc;
}

.btn{
    padding:12px 25px;
    background:#e50914;
    border:none;
    color:white;
    font-weight:600;
    cursor:pointer;
    border-radius:5px;
    transition:0.3s;
}

.btn:hover{
    background:white;
    color:#e50914;
}

/* Movies Section */
.movies{
    padding:60px;
}

.movies h3{
    margin-bottom:25px;
    font-size:26px;
}

.movie-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(200px,1fr));
    gap:25px;
}

.movie-card{
    background:#1c1c1c;
    border-radius:10px;
    overflow:hidden;
    transition:0.4s;
    cursor:pointer;
}

.movie-card img{
    width:100%;
    height:300px;
    object-fit:cover;
}

.movie-card:hover{
    transform:scale(1.07);
    box-shadow:0 0 20px rgba(229,9,20,0.6);
}

/* Footer */
footer{
    background:#000;
    text-align:center;
    padding:20px;
    margin-top:40px;
    color:#aaa;
}

/* Responsive */
@media(max-width:768px){
    nav{
        padding:15px 20px;
    }

    .hero{
        padding:20px;
        height:70vh;
    }

    .hero-content h2{
        font-size:35px;
    }

    .movies{
        padding:30px;
    }
}
</style>
</head>

<body>

<nav>
    <h1>MovieFlix</h1>
    <ul>
        <li>Home</li>
        <li>Movies</li>
        <li>Series</li>
        <li>Contact</li>
    </ul>
</nav>

<section class="hero">
    <div class="hero-content">
        <h2>Unlimited Movies, Anytime</h2>
        <p>Watch your favorite movies and shows in HD quality anytime, anywhere.</p>
        <button class="btn">Watch Now</button>
    </div>
</section>

<section class="movies">
    <h3>Popular Movies</h3>
    <div class="movie-grid">
        <div class="movie-card">
            <img src="https://images.unsplash.com/photo-1505685296765-3a2736de412f">
        </div>
        <div class="movie-card">
            <img src="https://images.unsplash.com/photo-1489599849927-2ee91cede3ba">
        </div>
        <div class="movie-card">
            <img src="https://images.unsplash.com/photo-1517602302552-471fe67acf66">
        </div>
        <div class="movie-card">
            <img src="https://images.unsplash.com/photo-1478720568477-152d9b164e26">
        </div>
    </div>
</section>

<footer>
    © 2026 MovieFlix | All Rights Reserved
</footer>

</body>
</html>
