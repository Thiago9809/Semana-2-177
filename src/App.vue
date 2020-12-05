<template>
  <div id="app">
    <div class="container-fluid" id="team">
      <div class="row justify-content-center mb-5">
        <div class="col mt-5" v-for="(item,index) of team"  :key="index">
          <team-card v-bind:member="item"></team-card>
        </div>
      </div>
    </div>
  </div>
</template>
npm run serv
<script>

import TeamCard from './components/TeamCard.vue'

export default {
  name: 'App',
  components:{
    TeamCard
  },
  
  data(){
    return{
      title: "Vivo dentro de Vue",
      team: [
        {
            codigo : 1 ,
            nombre : 'Santiago Herrera' ,
            descripcion : 'Lider de equipo y administrador de la mesa de servicios de TI, además, encargado de averiguar cómo se llevarán a cabo las actividades y luego garantizar que se realicen.' ,
            rol : 'Lider de equipo y administrador de la mesa de servicios de TI' ,
            image : '../img/Santiago.jpeg'
        },
        {
            codigo : 2 ,
            nombre : 'Daniel Rivera' ,
            descripcion : 'Jefe de Operaciones de Servicio, y me encargo de la gestión de incidencias, cumplimiento de solicitudes, gestión de acceso, gestión de eventos y gestión de problemas.' ,
            rol : 'Jefe de Operaciones de Servicio' ,
            image : '../img/Daniel.jpeg'
        },
        {
            codigo : 3 ,
            nombre : 'Felipe Medina' ,
            descripcion : 'Gerente de servicios de comunicaciones de TI, y el responsable del inicio de un nuevo servicio de TI junto con su transición a la producción y mantenimiento continuo.' ,
            rol : 'Gerente de servicios de comunicaciones' ,
            image : '../img/Felipe.jpeg'
        },
        {
            codigo : 4 ,
            nombre : 'Stiven Sabi' ,
            descripcion : 'Agente de servicios de TI y me encargo de tener los registros para demostrar que se han llevado a cabo las actividades apropiadas en los proyectos correspondientes.' ,
            rol : 'Agente de servicios de TI' ,
            image : '../img/Sabi.jpeg'
        },
      ]
    }
  }
}
</script>

