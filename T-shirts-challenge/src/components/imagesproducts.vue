<template>
  <div id="images">
      <ul id="photo">
          <li v-for="t in photos">
          <h4> {{ t.name }} </h4>
          <img :src="'./src/assets/' + t.img" alt="">
          <p> {{ t.price }} </p>
          </li>
      </ul>
  </div> 
</template>

<script>
export default {
    data() {
        return {
            photos:[
      { name: 'cbgb skull', img: 'cbgb.png', price: '20€' },
      { name: 'chemical', img: 'chemical.png', price: '35€' },
      { name: 'classic green', img: 'classicgreen.png', price: '29€' },
      { name: 'Harold Hunter', img: 'imagblanc.png', price: '32€' },
      { name: 'skateboard  lover', img: 'imagefonce.png', price: '10€' },
      { name: 'Consume', img: 'imagegrey.png', price: '20€' },
      { name: 'Super boo', img: 'superboo.png', price: '40€' },
      { name: 'College skull', img: 'tshirtnoir.png', price: '20€' },
      { name: 'Motor maniacs', img: 'motor.png', price: '33€' }
    ]
                
        }
        
    }
  
} 
</script>

<style lang="scss" scoped>
#images {
  width: 950px;
  background: #f1f3f5;
  height: auto;
  margin-right: 40px;
  border: 1px solid #EEE;
  border-radius: 5px;
  width: 700px;
  margin: 0px;


}
img {
    width: 120px;
    height: 120px;
}
#photo li {
    border: 1px solid #EEE;
    height: 120px;
    width: 170px;
    border-radius: 5px;
    height: auto;
    padding: 5px 0;
}
h4, p, h1 {
    padding: 0;
    margin: 0;
}

</style>


