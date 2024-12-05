<template>
  <div>
    <HeaderComponent :header="header" />
    <ExperienceComponent :experiences="experiences" />
    <EducationComponent :educations="educations" />
    <div class="grid grid-cols-3 gap-8 mt-8 pb-8">
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
        objective: `Soy un Desarrollador Full Stack con 3 años de experiencia, apasionado por la tecnología y graduado en Analista Programador Computacional. Me considero una persona motivada por el aprendizaje continuo, con un fuerte enfoque en la resolución de problemas y en la colaboración en equipo. Tengo una gran capacidad para adaptarme a nuevos desafíos y cambios, y me esfuerzo por mantenerme actualizado con las últimas tendencias tecnológicas.

A lo largo de mi carrera, he demostrado ser autodidacta y capaz de gestionar de manera efectiva mis tareas diarias, manteniendo una excelente capacidad de análisis y toma de decisiones. Me destaco por mi curiosidad, compromiso y responsabilidad, siempre buscando mejorar tanto en lo profesional como en lo personal.

Mi objetivo es seguir creciendo como profesional, aprender nuevas tecnologías y contribuir en proyectos innovadores y de alto impacto.`,
      }
      ],
      experiences: [
        {
          title: "Desarrollador Full Stack",
          company: "InverAndes SPA",
          location: "Santiago, Chile",
          dates: "2023-Noviembre - Presente",
          description: `Actualmente, me desempeño como desarrollador fullstack en InverAndes, donde trabajo en el desarrollo de una aplicación web que ofrece soluciones para la venta, el manejo de inventarios y la emisión de reportes. Para ello, utilizo tecnologías como Angular, C# .Net, PostgreSQL, Git, Insomnia y Bootstrap.
          
          Además, trabajo en el desarrollo de una aplicación móvil utilizando Flutter, Dart y Firebase, la cual se integra con la aplicación web. También soy responsable del despliegue de la aplicación tanto en Google Play Store como en Apple Store.

          Uno de los mayores desafíos que enfrenté en este proyecto fue aprender Angular en el menor tiempo posible, ya que, aunque conocía la tecnología, nunca había tenido la oportunidad de trabajar con ella. Sin embargo, pude aplicar los conocimientos adquiridos durante mi práctica con Flutter y Dart (en Hupaka) y con Vue.js en Analyze, lo que facilitó mi aprendizaje de Angular debido a la similitud con otros frameworks de JavaScript.`,
        },
        {
          title: "Desarrollador Full Stack",
          company: "Analyze",
          location: "Santiago, Chile",
          dates: "2021-Octubre - 2023-Abril",
          description: `Desarrollador fullstack para una empresa consultora, brindando soluciones informáticas personalizadas para diversas entidades privadas y públicas. Mi trabajo incluyó el desarrollo de aplicaciones web, así como la integración y consumo de APIs para optimizar los procesos. Utilicé tecnologías como Vue.js, PostgreSQL, Python, Django, Git, Jira y Postman, adaptándome a las necesidades de cada cliente y asegurando la entrega de soluciones a medida. `,
        },
        {
          title: "Desarrollador Móvil",
          company: "Hupaka",
          location: "Santiago, Chile",
          dates: "2021-Marzo - 2021-Julio",
          description: `Durante mi práctica profesional en Hupaka, me desempeñé como desarrollador de aplicaciones móviles, utilizando tecnologías como Flutter, Dart y Firebase. Uno de los mayores desafíos fue aprender de manera rápida y eficiente estas tecnologías, que eran nuevas para mí, pero con el tiempo logré dominar y utilizarlas para desarrollar una aplicación móvil robusta y funcional.

Además, no solo me encargué del desarrollo de la aplicación móvil, sino que también participé en la creación de la página web de la empresa, mejorando su presencia digital y optimizando la experiencia de usuario. Esta experiencia me permitió adquirir habilidades tanto en el desarrollo móvil como en el desarrollo web, brindándome una perspectiva más completa del ciclo de vida del software.

Gracias a mis resultados y compromiso, fui contratado por un periodo fijo, lo que me permitió seguir creciendo profesionalmente dentro de la empresa.`,
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
          title: "Educación Básica",
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
