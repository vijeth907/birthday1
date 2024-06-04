document.getElementById('birthdayForm').addEventListener('submit', function(event) {
    event.preventDefault();
    const name = document.getElementById('name').value;
    
    // Send name to GitHub using fetch API
    fetch('https://api.github.com/repos/your-username/your-repo/contents/names.txt', {
        method: 'PUT',
        headers: {
            'Authorization': 'token YOUR_GITHUB_TOKEN',
            'Content-Type': 'application/json'
        },
        body: JSON.stringify({
            message: 'Add new name',
            content: btoa(name) // encode name to base64
        })
    })
    .then(response => {
        if (response.status === 201 || response.status === 200) {
            document.getElementById('name').value = ''; // clear input field
            document.getElementById('thankYouMessage').style.display = 'block'; // show thank you message
        } else {
            alert('Error: ' + response.statusText);
        }
    })
    .catch(error => console.error('Error:', error));
});
