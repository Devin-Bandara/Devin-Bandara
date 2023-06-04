# Hi there 👋 I'm Devin Bandara

![giphy](https://github.com/Devin-Bandara/Devin-Bandara/assets/122140695/7324123d-8bab-4275-b22c-5c6f89c6670a)


- 🌱 I’m currently learning at the University of Moratuwa, Sri Lanka.
- 🌱 I’m currently learning Flutter and Node.js.
- 📫 How to reach me: devinmmcs@gmail.com
- ⚡ Fun fact: I love cooking.
- 💬 Ask me about anything!

## Technologies and Tools
<div style="display: flex; align-items: center;">
  <img src="https://img.icons8.com/color/48/000000/flutter.png" alt="Flutter" width="60" height="60">
  <img src="https://img.icons8.com/color/48/000000/nodejs.png" alt="Node.js" width="60" height="60">
  <img src="https://img.icons8.com/color/48/000000/html-5.png" alt="HTML/CSS" width="60" height="60">
  <img src="https://img.icons8.com/color/48/000000/javascript.png" alt="JavaScript" width="60" height="60">
  <img src="https://img.icons8.com/color/48/000000/java-coffee-cup-logo.png" alt="Java" width="60" height="60">
  <img src="https://img.icons8.com/color/48/000000/microsoft-sql-server.png" alt="Microsoft SQL" width="60" height="60">
  <img src="https://img.icons8.com/color/48/000000/mysql.png" alt="MySQL" width="60" height="60">
  <img src="https://img.icons8.com/color/48/000000/mongodb.png" alt="MongoDB" width="60" height="60">
  <img src="https://img.icons8.com/color/48/000000/c-programming.png" alt="C" width="60" height="60">
</div>

<!DOCTYPE html>
<html>
  <head>
    <title>My Profile</title>
    <style>
      .github-status {
        display: flex;
        flex-direction: column;
        align-items: center;
        font-family: Arial, sans-serif;
      }

      .github-status .emoji {
        font-size: 50px;
      }

      .github-status .message {
        margin-top: 10px;
      }
    </style>
  </head>
  <body>
    <div class="github-status">
      <h2>📊 GitHub Status:</h2>
      <div class="emoji"></div>
      <div class="message"></div>
    </div>

    <script src="https://unpkg.com/axios/dist/axios.min.js"></script>
    <script>
      const username = 'Devin-Bandara';

      axios
        .get(`https://api.github.com/users/${username}/status`)
        .then((response) => {
          const { data } = response;
          console.log('GitHub Status:', data);

          const emojiElement = document.querySelector('.emoji');
          const messageElement = document.querySelector('.message');

          if (data && data.status) {
            const { emoji, message } = data.status;
            emojiElement.textContent = emoji;
            messageElement.textContent = message;
          } else {
            emojiElement.textContent = '❌';
            messageElement.textContent = 'GitHub status not found.';
          }
        })
        .catch((error) => {
          console.error('Failed to fetch GitHub status:', error);

          const emojiElement = document.querySelector('.emoji');
          const messageElement = document.querySelector('.message');
          emojiElement.textContent = '❌';
          messageElement.textContent = 'Failed to fetch GitHub status.';
        });
    </script>
  </body>
</html>



<!--
**Devin-Bandara/Devin-Bandara** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
