<template>
  <div>
    <HeaderComponent :header="header" />
    <ExperienceComponent :experiences="experiences" />
    <EducationComponent :educations="educations" />
    <div class="grid grid-cols-3 gap-8 mt-8 ">
      <SkillsComponent class="border-r-2 border-indigo-300 pr-3" :skills="skills"/>
      <AptitudeComponent class="border-r-2 border-indigo-300 pr-3" :aptitudes="aptitudes"/>
      <LanguagesComponent :languages="languages"/>
    </div>
    
  </div>
</template>

<script>
import HeaderComponent from "./HeaderComponent.vue";
import ExperienceComponent from "./ExperienceComponent.vue";
import EducationComponent from "./EducationComponent.vue";
import SkillsComponent from "./SkillsComponent.vue";
import LanguagesComponent from "./LanguagesComponent.vue";
import AptitudeComponent from "./AptitudeComponent.vue";



export default {
  components: {
    HeaderComponent,
    ExperienceComponent,
    EducationComponent,
    SkillsComponent,
    LanguagesComponent,
    AptitudeComponent
  },
  data() {
    return {
      header:[
      {
        name:"Isaac Josue Vega Ferreira",
        jobTitle:"Analista Programador | Desarrollador Fullstack",
        address:"Camino costero KM 30, San Ignacio, Valdivia",
        phone:"+569 8254 4422",
        email:"ivega.josue@gmail.com",
        linkedin:"https://www.linkedin.com/in/isaac-vega-870153125/",
        github: "https://github.com/kvzon1984",
        objective: `Desarrollador Full Stack con 3 años de experiencia, apasionado por la tecnología, titulado de la carrera analista programador computacional, con ganas de aprender y trabajar en ambientes colaborativos en el desarrollo, poseo una muy buena voluntad para aprender y trabajar en equipo, con una rápida capacidad para la resolución de problemas, además una buena adaptación al cambio, autodidacta y en constante aprendizaje. 

        También poseo una alta capacidad para auto gestionar mis labores diarias y alta capacidad de análisis. Me considero una persona curiosa, comprometida y responsable, que busca Aprender y crecer Profesionalmente.`,
      }
      ],
      experiences: [
        {
          title: "Desarrollador Full Stack",
          company: "InverAndes SPA",
          location: "Santiago, Chile",
          dates: "2023-Noviembre - Presente",
          description: `Me desempeño como desarrollador fullstack para InverAndes, desarrollando una aplicación web.
          La cual da solución a la venta, manejo de inventario, emisión de reportes. Ocupando tecnologías como Angular, C# .Net, Posgre, Git, Insomnia, Azure. Bootstrap. 
          
          A su vez desarrollando una aplicación móvil utilizando tecnologías como Flutter, Dart, firebase la cual se conecta a la aplicación web. Encargado del despliegue tanto a play store como apple store. 

          Con el desafío de aprender angular lo antes posible ya que era una tecnología que si la habia oido pero sin la oportunidad de usarla, a su ves poniendo en practica los conocimientos adquiridos en mi practica Flutter y dart(Hupaka) y analyze ya que vue al ser un framework de JS no me costo tanto aprender Angular.`,
        },
        {
          title: "Desarrollador Full Stack",
          company: "Analyze",
          location: "Santiago, Chile",
          dates: "2021-Octubre - 2023-Abril",
          description: `Desarrollador fullstack para empresa consultora, para diferentes entidades privadas y publicas. 
          Orientada a soluciones informáticas a la medida de las necesidades.
          
          Utilizando tecnologías tales como: Vue, Postgres, Python, Django, Git, Jira, Postman. `,
        },
        {
          title: "Desarrollador Móvil",
          company: "Hupaka",
          location: "Santiago, Chile",
          dates: "2021-Marzo - 2021-Julio",
          description: `Realice mi practica profesional como desarrollador de aplicación móvil ocupando tecnología como Dart, flutter, Firebase. quedando contratado por un periodo fijo. 
          Con el gran desafío de tener que aprender lo antes posible una tecnología nueva como flutter y dart. `,
        },
      ],
      educations: [
        {
          title: "Analista Programador Computacional",
          institution: "Duoc UC",
          location: "Santiago, Chile",
          dates: "2019-Marzo - 2021-Junio",
        },
        {
          title: "Bootcamp Ruby on Rails",
          institution: "Desafio Latam",
          location: "Santiago, Chile",
          dates: "2017-Marzo - 2017-Mayo",
        },
        {
          title: "Educación Media",
          institution: "Colegio Bethel #3",
          location: "Santiago, Chile",
          dates: "1999 - 2002",
        },
        {
          title: "Educación Basuca",
          institution: "Colegio Chile | Colegio Bethel #3",
          location: "Santiago, Chile",
          dates: "1998 - 1991",
        },
      ],
      skills: [
        ".NET", "JavaScript", "TypeScript", "AngularJS", "PostgreSQL", "Firebase",
        "Dart", "Flutter", "Vue", "React", "Git", "SQL", "HTML", "CSS", "Python",
        "Django", "Ubuntu",
      ],
      aptitudes: [
        "Proactivo", "Responsable", "Comprometido",
      ],
      languages: [
        { name: "Español", level: "Nativo" },
        { name: "Inglés", level: "Nivel Básico" },
      ],
    };
  },
};
</script>
