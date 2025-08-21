# kangen-website
body {
    font-family: 'Roboto', sans-serif;
    margin:0;
    padding:0;
    background:#f4f4f9;
    color:#333;
}

header {
    background: linear-gradient(135deg, #9b59b6, #bdc3c7);
    color:white;
    text-align:center;
    padding:60px 20px;
}

header h1 {
    font-size:3rem;
    margin:10px 0;
}

header p {
    font-size:1.2rem;
    max-width:700px;
    margin: 0 auto;
}

header .banner {
    max-width:100%;
    border-radius:10px;
    margin-bottom:20px;
}

main {
    max-width:1200px;
    margin:40px auto;
    padding:0 20px;
}

section {
    background:white;
    padding:30px;
    margin-bottom:40px;
    border-radius:10px;
    box-shadow:0 4px 12px rgba(0,0,0,0.1);
}

section h2 {
    color:#9b59b6;
    font-size:2rem;
    margin-bottom:20px;
}

section p, section ul {
    font-size:1rem;
    line-height:1.6;
}

section ul {
    list-style-type: disc;
    margin-left:20px;
}

.water-types {
    display:flex;
    flex-wrap:wrap;
    gap:20px;
}

.water-box {
    flex:1 1 calc(20% - 20px);
    background:#fdfdfd;
    border-radius:8px;
    padding:10px;
    text-align:center;
    box-shadow:0 4px 8px rgba(0,0,0,0.1);
    cursor: pointer;
    transition: transform 0.3s, box-shadow 0.3s;
    position: relative;
    opacity: 0;
    transform: translateY(50px);
}

.water-box:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.2);
}

.product-box {
    flex:1 1 calc(33% - 20px);
    background:#fdfdfd;
    border-radius:8px;
    padding:10px;
    text-align:center;
    box-shadow:0 4px 8px rgba(0,0,0,0.1);
    cursor: pointer;
    transition: transform 0.3s, box-shadow 0.3s;
    position: relative;
    opacity: 0;
    transform: translateY(50px);
}

.product-box:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.2);
}

.water-box.show, .product-box.show {
    opacity: 1;
    transform: translateY(0);
}

.water-box img, .product-box img {
    max-width:100%;
    border-radius:6px;
    margin-bottom:10px;
}

.description {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.3s, opacity 0.3s;
    opacity: 0;
}

.water-box:hover .description,
.product-box:hover .description {
    max-height: 100px;
    opacity: 1;
}

.faq {
    max-width: 800px;
    margin: 0 auto;
}

.faq-item {
    margin-bottom: 15px;
    border-radius: 6px;
    overflow: hidden;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

.faq-question {
    width: 100%;
    padding: 15px;
    text-align: left;
    background: #9b59b6;
    color: white;
    border: none;
    cursor: pointer;
    font-size: 1.1rem;
    transition: background 0.3s;
}

.faq-question:hover {
    background: #732d91;
}

.faq-answer {
    max-height: 0;
    overflow: hidden;
    background: #fdfdfd;
    padding: 0 15px;
    transition: max-height 0.3s ease, padding 0.3s ease;
}

.faq-answer p {
    margin: 10px 0;
}

footer {
    background:#9b59b6;
    color:white;
    text-align:center;
    padding:20px;
}

footer a {
    color:white;
    text-decoration:underline;
}

footer h3 {
    margin-top: 30px;
    color: white;
}

footer form {
    margin-top: 15px;
    max-width: 400px;
    margin-left: auto;
    margin-right: auto;
}

footer input, footer textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    border-radius: 6px;
    border: 1px solid #ccc;
}

footer button.btn {
    width: 100%;
    background:#8e44ad;
    border:none;
    padding:12px;
    font-size:1rem;
    cursor:pointer;
}

footer button.btn:hover {
    background:#732d91;
}

.btn {
    display:inline-block;
    background:#9b59b6;
    color:white;
    padding:10px 20px;
    border-radius:6px;
    margin-top:10px;
    text-decoration:none;
}

@media(max-width:992px){
    .water-box { flex:1 1 calc(50% - 20px); }
    .product-box { flex:1 1 calc(50% - 20px); }
}

@media(max-width:600px){
    .water-box, .product-box { flex:1 1 100%; }
    header h1{font-size:2.2rem;}
    header p{font-size:1rem;}
    section h2{font-size:1.6rem;}
}
