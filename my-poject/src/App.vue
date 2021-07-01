<template>
  <div class="container">
    <Header title="プロフィール" />
    <Profiles subtitle="基本情報" />

  </div>
  

</template>

<script>
import Header from './components/Header'
import Profiles from './components/Profiles'


export default {
  name: 'App',
  components: {
    Header,
    Profiles,
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=M+PLUS+Rounded+1c:wght@700&family=Poppins:wght@300&display=swap');


* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: 'Poppins', sans-serif;
}
.container {
  max-width: 500px;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 1px solid steelblue;
  padding: 30px;
  border-radius: 5px;
}
.btn {
  display: inline-block;
  background: #000;
  color: #fff;
  border: none;
  border-radius: 5px;
  padding: 10px 20px;
  margin: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}
</style>
