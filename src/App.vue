<template>
<div align="center">
  <h1>{{ titulo }}</h1>

  <ul :id="fotos.id">
    <li v-for="foto of fotos" >
      <img :src="fotos.url" :alt="fotos.titulo">
    </li>
  </ul>  

</div>
</template>

<script>
export default {
  
  data() {
    return {

      titulo: 'STOP-MOTION',
      fotos: [
        {
          url: 'https://www.wheretraveler.com/sites/default/files/images/pizzad.jpg',
          titulo: 'stopMotion',
          id: 'foto1',
        },
        {
          url: 'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.gannett-cdn.com%2Fpresto%2F2020%2F03%2F02%2FPDTN%2Fd8f03277-3956-4d29-83a7-ee8a592290ed-PP_-_Deep_Dish_Detroit_Style.jpg%3Fcrop%3D2999%2C1687%2Cx0%2Cy277%26width%3D2999%26height%3D1687%26format%3Dpjpg%26auto%3Dwebp&f=1&nofb=1',
          titulo: 'stopMotion',
          id: 'foto2',
        }
      ]
    }
  }
}
</script>

<style lang="scss">

</style>
