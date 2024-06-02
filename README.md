<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Animal Image Display</title>
</head>
<body>

<h2>Enter the first letter of your name:</h2>
<input type="text" id="letterInput">
<button onclick="displayAnimal()">Display Animal</button>

<div id="animalImage"></div>

<script>
function displayAnimal() {
    var letter = document.getElementById("letterInput").value.toLowerCase();
    var animalImage = document.getElementById("animalImage");

    switch(letter) {
        case 'a':
            animalImage.innerHTML = '<img src="https://www.example.com/animal_a.jpg" alt="Animal A">';
            break;
        case 'b':
            animalImage.innerHTML = '<img src="https://www.example.com/animal_b.jpg" alt="Animal B">';
            break;
        // Add more cases for other letters and corresponding animal images
        default:
            animalImage.innerHTML = '<p>No animal found for that letter.</p>';
    }
}
</script>

</body>
</html>
