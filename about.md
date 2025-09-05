---
layout: page
permalink: /about
nav_order: 1
---


# About
3rd year student at UCL in mathematics with interest in logic, computability, and philosophy. I'm looking to eventually do a PhD in mathematical logic. I basically like anything complex, but also am a big fan of beer, midwest-emo music, and cycling. Here are my top 5 songs in the last 3 months: 


### 🎵 My Top 5 Songs (Last 3 Months)

<div id="top-tracks">Loading...</div>

<script>
  const apiKey = "503ee6ce06f4bf25df8dac6f986aac51";  // replace with your key
  const username = "hamtser"; // replace with your username
  const url = `https://ws.audioscrobbler.com/2.0/?method=user.getTopTracks&user=${username}&period=3month&limit=5&api_key=${apiKey}&format=json`;

  fetch(url)
    .then(response => response.json())
    .then(data => {
      const tracks = data.toptracks.track;
      let html = "<ol>";
      tracks.forEach(track => {
        html += `<li>
          <strong>${track.name}</strong> by ${track.artist.name} 
          (${track.playcount} plays)
        </li>`;
      });
      html += "</ol>";
      document.getElementById("top-tracks").innerHTML = html;
    })
    .catch(error => {
      document.getElementById("top-tracks").innerText = "Failed to load tracks 😢";
      console.error(error);
    });
</script>



# Contact
UCL Email: <archie.worth.23@ucl.ac.uk>\\
Personal Email: <archie.worth7@gmail.com>

<img style="float:bottom; margin-bottom:10px; width:300px; height:auto;"
     src="{{ site.baseurl }}/assets/img/cwoffee.png" 
     alt="Cwoffee" 
     class="bottom-img"
/>

