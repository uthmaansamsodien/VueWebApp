<template>
  <div id="displayss">
    
  </div>
</template>

<script>
export default {

}

async function getPlayers(){
      const data = await fetch('https://uthmaansamsodien.github.io/JsonServerToo/user.json')
      const formatData = await data.json()
      let playerData = formatData.players
      const display = document.querySelector('#displayss')
      playerData.forEach(players =>{
      display.innerHTML += `
      <div class="card">
          <div class="card-body">
            <h3 class="card-title">${players.firstName} ${players.Surname}</h3>
            <p class="card-text">${players.Age}</p>
          </div>
        </div>
    `
  })
  }
    getPlayers()

</script>

<style>
.card{ 
  padding: 3rem;
}
</style>