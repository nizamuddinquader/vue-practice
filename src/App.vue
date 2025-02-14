<script setup>
  const persons = [
    {
      image:'https://images.unsplash.com/photo-1557862921-37829c790f19?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8bWFufGVufDB8fDB8fHww',
      name:'Jonas Kakaroto',
      title:'Photographer',
      id:'1'
    },
    {
      image:'https://media.istockphoto.com/id/1867533396/photo/young-asian-man-using-smart-phone-in-cafe.webp?a=1&b=1&s=612x612&w=0&k=20&c=_Bal1cuuXVr3luD6LkQkLkgNmqkV2WS_03M1d9Spez4=',
      // image:'./assets/images/designer.jpg',
      name:'John Doe ',
      title:'Software Engineer',
      id:'2'
    },
    {
      image:'https://media.istockphoto.com/id/2172317014/photo/happy-hispanic-man-working-on-laptop-at-home.webp?a=1&b=1&s=612x612&w=0&k=20&c=05ojo1QnTTyuFif76-P2mTmhwl4jg8t19aoxAzSB_B8=',
      name:'Charlie Green',
      title:'Designer',
      id:'3'
    }
]


</script>

<template>
  <div class="container mt-5">
    <div class="row">
      <div class="col-md-12">
        <div class="card mt-5 border-4">
          <h1 class="text-center mt-3">Team Members</h1>
          <p class="text-center">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Corporis, libero.</p>
          <div class="card-body mt-3">
            <div class="row">
              <!-- <div class="col-md-4" v-for="person in persons" :key="person.id"> -->
              <div class="col-md-4" v-for="(person, index) in persons" :key="person.id">
                <!-- <img :src="person.image" class="w-100 img-fluid" :class="person.id==2?'h-75':'h-50'" alt="team-member-photo"> -->
                <img :src="person.image" class="w-100 img-fluid" :class="index==1?'h-75':'h-50'" alt="team-member-photo">
                <h4 class="mt-3" >{{ person.name }}</h4>
                <p>{{ person.title }}</p>
              </div>
              <!-- <div class="col-md-4">
                <img :src="persons[1].image" class="w-100 h-50 img-fluid" alt="team-member-photo">
                <h4>{{ persons[1].name }}</h4>
                <p>{{ persons[1].title }}</p>
              </div> -->
              <!-- <div class="col-md-4">
                <img :src="persons[2].image" class="w-100 h-50 img-fluid" alt="team-member-photo">
                <h4>{{ persons[2].name }}</h4>
                <p>{{ persons[2].title }}</p>
              </div> -->
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>