<template>
  <div class="Calendar">
    <router-link to="/"><b-icon icon="x" class="back" style="width: 30px; height: 30px; float: right; margin-right: 0.4em; height: 100%; color: black;"></b-icon></router-link>          

    <h2>* september</h2> 

    <b-table striped hover :items="items"></b-table>
    
    <router-link to="/Maps">
      <p class="loc"><b-icon icon="geo-alt-fill" scale="2" style="color: #b0c8f3" animation="cylon-vertical"></b-icon></p>
    </router-link>

  </div>
    
</template>


<script>
import info from "../data.js"

export default {
    name: 'Calendar',
    props: ['calendar'],
    data: function(){
    return {
      partidos: null,
      items: [
          { day: 1, time: '9:30 a.m.', teams: 'U1 vs. U4', location: 'AJ K' },
          { day: 1, time: '1.00 p.m.', teams: 'U3 vs. U2', location: 'Greenbay' },
          { day: 8, time: '0.30 a.m.', teams: 'U5 vs. U6', location: 'Howard AY' },
          { day: 15, time: '1.00 p.m.', teams: 'U6. vs. U1', location: 'Marjorie PH' },
          { day: 15, time: '9:30 a.m.', teams: 'U2 vs. U4', location: 'North' },
          { day: 22, time: '1.00 p.m.', teams: 'U3 vs. U5', location: 'AJ K' },
          { day: 22, time: 'Geneva', teams: 'U1 vs. U3', location: 'South' },]
    }
  },
  methods: {
    getMonths: function(){
      this.partidos = info.match
      console.log(this.partidos)
    }
  },
  created (){
      this.getMonths()
  }
}
</script>

<style>

.loc{
  text-align: right;
  margin-right: 1.5em;
}
</style>
