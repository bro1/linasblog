---
date: 2024-11-01T01:00:35.745+13:00
author: Linas
summary: My often used links
categories:
  - posts
title: My iHeartRadio music links
tags:
  - links

---

<style>
.container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
}
.btn {
    background-color: #dddddd;    
    padding: 5px;
    margin: 5px;
    height: 90%;
    text-align: center;
}

</style>


<div id="iheart" class="container">
</div>


<script>

function shuffleArray(array) {
  for (let i = array.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [array[i], array[j]] = [array[j], array[i]];
  }
  return array;
}

function renderMusicArtistsHTML(artistsData) {
  const shuffledArtists = shuffleArray([...artistsData]);
  return shuffledArtists.map(artist => {
    return `<a href="${artist.url}" target="_blank"><div class="btn">${artist.title}</div></a>`;
  }).join('');
}


const musicArtists = [
  {
    "title": "Ed Guy",
    "url": "https://www.iheart.com/artist/edguy-4953/"
  },
  {
    "title": "The Prodigy",
    "url": "https://www.iheart.com/artist/the-prodigy-37121/"
  },
  {
    "title": "Fatboy slim",
    "url": "https://www.iheart.com/artist/fatboy-slim-29305/"
  },
  {
    "title": "CSS",
    "url": "https://www.iheart.com/artist/css-86492/"
  },
  {
    "title": "Chemical brothers",
    "url": "https://www.iheart.com/artist/the-chemical-brothers-27831/"
  },
  {
    "title": "Sisters of Mercy",
    "url": "https://www.iheart.com/artist/the-sisters-of-mercy-75773/"
  },
  {
    "title": "Cage the elephant",
    "url": "https://www.iheart.com/artist/cage-the-elephant-117804/"
  },
  {
    "title": "Andrew WK",
    "url": "https://www.iheart.com/artist/andrew-w-k-39618/"
  },
  {
    "title": "Beck",
    "url": "https://www.iheart.com/artist/beck-11447/"
  },
  {
    "title": "Gorillaz",
    "url": "https://www.iheart.com/artist/gorillaz-29588/"
  },
  {
    "title": "Nirvana",
    "url": "https://www.iheart.com/artist/nirvana-40473/"
  },
  {
    "title": "Sublime",
    "url": "https://www.iheart.com/artist/nirvana-40473/"
  },
  {
    "title": "Gnarls Barkley",
    "url": "https://www.iheart.com/artist/gnarls-barkley-58770/"
  },
  {
    "title": "Kaleo",
    "url": "https://www.iheart.com/artist/kaleo-352537/"
  },
  {
    "title": "Bishop briggs",
    "url": "https://www.iheart.com/artist/bishop-briggs-31199070/"
  },
  {
    "title": "Kongos",
    "url": "https://www.iheart.com/artist/kongos-771253/"
  },
  {
    "title": "The Black Keys",
    "url": "https://www.iheart.com/artist/the-black-keys-9288/"
  },
  {
    "title": "The Raconteurs",
    "url": "https://www.iheart.com/artist/the-raconteurs-58373/"
  },
  {
    "title": "Cake",
    "url": "https://www.iheart.com/artist/cake-70491/"
  },
  {
    "title": "The Presidents of the United States",
    "url": "https://www.iheart.com/artist/the-presidents-of-the-united-states-131862/"
  },
  {
    "title": "Bloodhound Gang",
    "url": "https://www.iheart.com/artist/bloodhound-gang-39404/"
  },
  {
    "title": "The Offspring",
    "url": "https://www.iheart.com/artist/the-offspring-80925/"
  },
  {
    "title": "The Flaming Lips",
    "url": "https://www.iheart.com/artist/the-flaming-lips-33830/"
  },
  {
    "title": "Liquido",
    "url": "https://www.iheart.com/artist/liquido-3602/"
  },
  {
    "title": "Shiny Toy Guns",
    "url": "https://www.iheart.com/artist/shiny-toy-guns-6345/"
  },
  {
    "title": "Maneskin",
    "url": "https://www.iheart.com/artist/maneskin-31997005/"
  },
  {
    "title": "Smash Mouth",
    "url": "https://www.iheart.com/artist/smash-mouth-39146/"
  },
  {
    "title": "Bowling for Soup",
    "url": "https://www.iheart.com/artist/bowling-for-soup-57672/"
  },
  {
    "title": "Ladytron",
    "url": "https://www.iheart.com/artist/ladytron-182332/"
  },
  {
    "title": "Tocotronic - Gehen die Leute",
    "url": "https://www.iheart.com/artist/tocotronic-207585/songs/gehen-die-leute-125048587/"
  },
  {
    "title": "Tocotronic",
    "url": "https://www.iheart.com/artist/tocotronic-207585/"
  },
  {
    "title": "The BossHoss",
    "url": "https://www.iheart.com/artist/the-bosshoss-30295187/"
  },
  {
    "title": "Johnny Cash",
    "url": "https://www.iheart.com/artist/johnny-cash-1616/"
  },
  {
    "title": "Nine Inch Nails",
    "url": "https://www.iheart.com/artist/nine-inch-nails-40022/"
  },
  {
    "title": "R.E.M.",
    "url": "https://www.iheart.com/artist/rem-3610/"
  },
  {
    "title": "Drugstore",
    "url": "https://www.iheart.com/artist/drugstore-126197/"
  },
  {
    "title": "Rob Dougan",
    "url": "https://www.iheart.com/artist/rob-dougan-98589/"
  },
  {
    "title": "Flight of the Conchords",
    "url": "https://www.iheart.com/artist/flight-of-the-conchords-98661/"
  },
  {
    "title": "Radiohead",
    "url": "https://www.iheart.com/artist/radiohead-974/"
  },
  {
    "title": "Biplan",
    "url": "https://www.iheart.com/artist/biplan-633878/albums/braks-55327560/"
  },
  {
    "title": "The Crystal Method",
    "url": "https://www.iheart.com/artist/the-crystal-method-11521/"
  },
  {
    "title": "Colony House",
    "url": "https://www.iheart.com/artist/colony-house-30401248/songs/cannonballers-184575821/"
  },
  {
    "title": "Alice in Videoland",
    "url": "https://www.iheart.com/artist/alice-in-videoland-141425/"
  },
  {
    "title": "Lana Del Rey",
    "url": "https://www.iheart.com/artist/lana-del-rey-692502/songs/say-yes-to-heaven-217591471/"
  },
  {
    "title": "The Last Dinner Party",
    "url": "https://www.iheart.com/artist/the-last-dinner-party-40240530/"
  },
  {
    "title": "Live - All Over You",
    "url": "https://www.iheart.com/artist/live-41289/songs/all-over-you-76445055/"
  },
  {
    "title": "Ash",
    "url": "https://www.iheart.com/artist/ash-30704131/"
  },
  {
    "title": "Goldfrapp",
    "url": "https://www.iheart.com/artist/goldfrapp-29488/"
  },
  {
    "title": "Rage Against the Machine",
    "url": "https://www.iheart.com/artist/rage-against-the-machine-89499/"
  },
  {
    "title": "East River Pipe - Summer Boy",
    "url": "https://www.iheart.com/artist/east-river-pipe-281491/songs/summer-boy-128349345/"
  }
];

const musicArtistsHTML = renderMusicArtistsHTML(musicArtists);
document.getElementById('iheart').innerHTML = musicArtistsHTML;

</script>


