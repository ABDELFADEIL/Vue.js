<template>
  <div id="sidebar"> 
      <input type="reset" value="reset filter">
      <hr class="hr1">
      <p class="price">Price max</p>
      <input v-model="leprix" id="valinpt" type="text" placeholder="enter le prix" value="" min="0" max="50" step="5">
      <p class="prix">{{leprix}} €</p>
      <hr>
      <h5 id="brands">Brands</h5>
      <div class="check">
           <div>  <input v-model="inval" type="checkbox" id="" value=""> <label for=""> obye       </label> </div>
           <div>  <input v-model="inval" type="checkbox" id="" value=""> <label for=""> zoo york   </label> </div>
           <div>  <input v-model="inval" type="checkbox" id="" value=""> <label for=""> the kooples</label> </div>
           <div>  <input v-model="inval" type="checkbox" id="" value=""> <label for=""> element    </label> </div>
           <div>  <input v-model="inval" type="checkbox" id="" value=""> <label for=""> cbgb       </label> </div>
           <div>  <input v-model="inval" type="checkbox" id="" value=""> <label for=""> dickies    </label> </div>
      </div>
      <hr>
      <h5>Colors</h5>
      <div class="couleurs">
        <div id="black"></div>
        <div id="white"></div>
        <div id="grey"></div>
        <div id="red"></div>
        <div id="yellowgreen"></div>
        <div id="green"></div>
      </div>



     </div>      
</template>
<script>
export default {
   

}
</script>

<style lang="scss" scoped>
#sidebar {
    color: black;
    border: 1 px solid black;
    border-radius: 5px;
    width: 400px;
    height: 500px;
    background: #f1f3f5;
    margin-left: 0;
    margin-right: 30px;
}
h5 {
  display: block;
  float: left;
  padding-left: 20px; 
  width: 100%;
  text-align: left; 
}
.check {
  text-align: left;
  margin-left: 10px;

}
.check input[type=checkbox] {
  text-align: right;
  margin-right: 20px;
}
input[type=reset] {
  float: left;
  margin: 10px;
  width: 80px;
  margin-right: 200px;
}
.hr1 {
  width: 98%;
  float: left;
}
.price {
  float: left;
  width: 100%;
}
// .check input:nth-of-type(1) {
//   text-align: center;
//   margin-left: 60px;
// }
.couleurs {
  display: flex;
  flex-flow: row wrap;
  width: 350px;
  justify-content: space-between;
  margin-left: 20px; 
}
.couleurs > div {
  width: 40px;
  height: 40px;
  border: 1px solid black;
}
.couleurs #black {
  background: black;
}
.couleurs #white {
  background: white;
}
.couleurs #grey {
  background: grey;
}
.couleurs #red {
  background: red;
}
.couleurs #yellowgreen {
  background: yellowgreen;
}
.couleurs #green {
  background: green;
}
</style>


