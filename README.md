<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Valentine Day</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <br><br><br><br><br><br>
    <header>
      <div class="main-container">
       <h1>Happy Valentine's Day</h1>
      </div>
    </header>


    <div class="container">
        <h2>Masukan Password!</h2>
        <div class="keypad">
            <input type="password" id="passwordInput" placeholder="Masukkan Tanggal Kita" disabled>
            <div class="number-grid">
                <!-- angka angka tabel-->
                <button onclick="addNumber (1)">1</button>
                <button onclick="addNumber (2)">2</button>
                <button onclick="addNumber (3)">3</button>
                <button onclick="addNumber (4)">4</button>
                <button onclick="addNumber (5)">5</button>
                <button onclick="addNumber (6)">6</button>
                <button onclick="addNumber (7)">7</button>
                <button onclick="addNumber (8)">8</button>
                <button onclick="addNumber (9)">9</button>
                <button onclick="clearPassword()">Clear</button>
                <button onclick="addNumber (0)">0</button>
                <button onclick="checkPassword()">OK</button>
            </div>
        </div>
        <p id="message"></p>
    </div>
    
    <script src="script.js"></script>
</body>
</html>

header h1 {
    display: flex;
    align-items: center;
    justify-content: center;
}

body {
    background-color: gray;
}

.container {
    
    width: 100%;
    max-width: 400px;
    margin: 0 auto;
    background-color: white;
    text-align: center;
    display: flex;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 0 10px rgb(0, 0, 0, 0.1);
}

.container h2 {
    display: flex;
    align-items: center;
}

.keypad {
    margin-top: 20px;
}

.number-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
    justify-content: center;
    width: 100%;
    max-width: 800px;
}

button {
    padding: 15px;
    width: 100%;
    font-size: 18px;
    border: none;
    background-color: #007bff;
    color: white;
    border-radius: 4px;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
}

input {
    width: 200px;
    padding: 10px;
    text-align: center;
    margin-bottom: 10px;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 18px;
}



@media screen and (max-width: 1000px) {
  

input {
    width: 65%;
}

.container h2 {
    font-size: 1rem;
}

.container {
    box-shadow: 0 0 10px rgb(0, 0, 0, 0.1);
    width: 85%;
}

}
