![](Workhard.gif)

### Hi there, I'm Gabriel - aka Horizon

## I'm currently training to become a web developer at Simplon

- At the moment, I'm working on: Beesafe, a web application to prevent the person from finding themselves in dangerous situations.
- I’m currently learning: Php and javascript.
- I’m looking to collaborate on: any interesting open source project.
- I’m looking for help with: understanding what the hell I'm doing.
- How to reach me: add Horizon#6417 on discord
- i dont know everything but i try to learn fast 


<div class="github-card">
  <h2>Stats GitHub de GabrielHori</h2>
  <ul id="stats">
    <li>Repos publics: <span id="repos"></span></li>
    <li>Commits: <span id="commits"></span></li>
    <li>Followers: <span id="followers"></span></li>
  </ul>
</div>

<script>
  const username = "GabrielHori";

  fetch(`https://api.github.com/users/${username}`)
    .then(res => res.json())
    .then(data => {
      document.getElementById("repos").innerText = data.public_repos;
      document.getElementById("followers").innerText = data.followers;
    });

  fetch(`https://api.github.com/users/${username}/events/public`)
    .then(res => res.json())
    .then(events => {
      const commitCount = events.filter(e => e.type === "PushEvent").length;
      document.getElementById("commits").innerText = commitCount;
    });
</script>

<style>
  .github-card {
    padding: 20px;
    border-radius: 12px;
    background-color: #1e1e2f;
    color: #fff;
    width: 250px;
    font-family: sans-serif;
  }
  .github-card h2 { font-size: 18px; margin-bottom: 10px; }
  .github-card ul { list-style: none; padding: 0; }
  .github-card li { margin: 6px 0; }
</style>


