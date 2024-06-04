<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>User Response Storage</title>
</head>
<body>
<h1>Enter Your Response</h1>
<form id="responseForm">
  <label for="userResponse">Your Response:</label><br>
  <input type="text" id="userResponse" name="userResponse"><br><br>
  <button type="submit">Submit</button>
</form>

<script>
document.getElementById("responseForm").addEventListener("submit", function(event){
  event.preventDefault();
  var userResponse = document.getElementById("userResponse").value;
  localStorage.setItem("userResponse", userResponse);
  alert("Response stored successfully!");
});
</script>

</body>
</html>
