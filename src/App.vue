<template>
  <div>
    <h2 >{{title}}</h2>
    <div :key="user" v-for="user in users" class="nav">{{user.index}} My name is {{user.name}} and surname {{user.surname}} I work at company called '{{user.company}}'</div>
    <!-- npm run serve -->
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      title: "Типо список",
      users: [{index:'1',name:'Tom',surname:'Redl',company:'Hogwarts'},
      {index:'2',name:'Egor',surname:'Letov',company:'Windows'},
      {index:'3',name:'Chu ',surname:'Yong',company:'Interpreters'}]
    };


   }  
};
</script>
<style>
div.active {
    color: red;
}
</style>
