---
layout: page
permalink: /about
nav_order: 1
---


# About
3rd year student at UCL in mathematics with interest in logic, computability, and philosophy. I'm looking to do eventually do a PhD in mathematical logic. I basically like anything complex, but also am a big fan of beer, midwest-emo music, and cycling. Here is the last 5 songs I've listened to: 

<div id="lastfm-tracks">Loading…</div>

<script>
const apiKey = "503ee6ce06f4bf25df8dac6f986aac51";   // replace with your API key
const user   = "hamtser";  // replace with your Last.fm username

fetch(`https://ws.audioscrobbler.com/2.0/?method=user.getrecenttracks&user=${user}&limit=5&api_key=${apiKey}&format=json`)
  .then(res => res.json())
  .then(data => {
    const tracks = data.recenttracks.track;
    let html = "<ul>";
    tracks.forEach(track => {
      html += `<li>
        <strong>${track.artist['#text']}</strong> — ${track.name}
      </li>`;
    });
    html += "</ul>";
    document.getElementById("lastfm-tracks").innerHTML = html;
  })
  .catch(err => {
    document.getElementById("lastfm-tracks").innerHTML = "⚠️ Failed to load Last.fm data.";
    console.error(err);
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

