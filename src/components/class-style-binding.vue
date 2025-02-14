<script setup>
  const bg = {
    bPrimary:'bg-primary',
    bSecondary:'bg-secondary',
    bSuccess:'bg-success'
}



  // const border = {
  //   borderTop: '2px solid red'
  // }

  const bRed = 'border-top:3px solid red'
  const bTeal = 'border-top:3px solid teal'
    
  const messageType = true

   
  const bgColor = {
    backgroundColor:'black'
  } 

  const bgcColorChange = "error"

  if("error"==bgcColorChange){
    bgColor.backgroundColor ='red'
    bgColor.color = 'black'
    bgColor.fontSize = '20px'
    bgColor.borderLeft = '2px solid black'
    bgColor.borderRight = '2px solid black'
    bgColor.fontWeight = '500'

  }


</script>

<template>
  
    <div class="container">
      <div class="row">
        <div class="col-md-12 d-flex justify-content-center mt-5 text-white p-0">
          <div class=" p-3 " :class="bg.bPrimary">I am col 1, Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sint, excepturi!</div>
          <div class=" p-3 me-5 ms-5 " :class="bg.bSecondary">I am col 2, Lorem ipsum, dolor sit amet consectetur adipisicing elit. Tempore, animi!</div>
          <div class=" p-3 " :class="bg.bSuccess">I am col 3, Lorem ipsum dolor sit, amet consectetur adipisicing elit. Modi, impedit!</div>
        </div>
      </div>
    </div>

  <div class="container">
    <div class="row">
      <div class="col-md-12 d-flex justify-content-center mt-5 text-white text-center p-0">
        <div class="p-3 flex-grow-1 p=0" :style="bgColor">I am col 12, Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sint, excepturi!</div>
      </div>
    </div>
  </div>

  <div class="container">
    <div class="row">
      <!-- <div class="col-md-12 d-flex justify-content-center mt-5 text-dark text-center p-0">
        <div class="bg-warning p-3 flex-grow-1" :style="messageType==true?bRed:bTeal">I am col 12, Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sint, excepturi!</div>
      </div> -->
      <!-- <div class="col-md-12 d-flex justify-content-center mt-5 text-dark text-center p-0">
        <div class="bg-warning p-3 flex-grow-1" :style="[messageType==true?bRed:bTeal,messageType==true?'font-size:18px':'font-size:24px']">I am col 12, Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sint, excepturi!</div>
      </div> -->
      <div class="col-md-12 d-flex justify-content-center mt-5 text-dark text-center p-0">
        <div class="bg-warning p-3 flex-grow-1" :style="messageType==true?[bRed,'font-size:18px']:[bTeal,'font-size:24px']">I am col 12, Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sint, excepturi!</div>
      </div>
      <!-- <div class="col-md-12 d-flex justify-content-center mt-5 text-dark text-center p-0" :style="border">
        <div class="bg-warning p-3 flex-grow-1">I am col 12, Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sint, excepturi!</div>
      </div> -->
    </div>
  </div>
 
  


</template>

<style scoped>

</style>