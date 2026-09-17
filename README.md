<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>GitHub Profile</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .card {
      background: white;
      width: 420px;
      border-radius: 16px;
      padding: 24px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.1);
      text-align: center;
    }
    img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      border: 3px solid #ddd;
    }
    h2 {
      margin: 12px 0 6px;
    }
    .username {
      color: #666;
      margin-bottom: 12px;
    }
    .bio {
      color: #444;
      margin-bottom: 16px;
    }
    a {
      text-decoration: none;
      background: #24292f;
      color: white;
      padding: 10px 16px;
      border-radius: 8px;
      display: inline-block;
    }
    .stats {
      display: flex;
      justify-content: space-between;
      margin-top: 20px;
      font-size: 14px;
      color: #444;
    }
  </style>
</head>
<body>
  <div class="card" id="profile"></div>

  <script>
    const username = "takpiyush10-maker";

    fetch(`https://api.github.com/users/${username}`)
      .then(response => response.json())
      .then(data => {
        if (data.message) {
          document.getElementById("profile").innerHTML = "<p>User not found</p>";
          return;
        }

        document.getElementById("profile").innerHTML = `
          <img src="${data.avatar_url}" alt="${data.login}">
          <h2>${data.name || data.login}</h2>
          <div class="username">@${data.login}</div>
          <div class="bio">${data.bio || "No bio available"}</div>

          <div class="stats">
            <div>Followers: ${data.followers}</div>
            <div>Following: ${data.following}</div>
            <div>Repos: ${data.public_repos}</div>
          </div>

          <br>
          <a href="${data.html_url}" target="_blank">View GitHub Profile</a>
        `;
      })
      .catch(error => {
        document.getElementById("profile").innerHTML = "<p>Something went wrong</p>";
        console.error(error);
      });
  </script>
</body>
</html>
