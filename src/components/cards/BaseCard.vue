<template>
<el-row :gutter="12">
  <el-col class="BaseCard" :span="5" v-for="card in cardOp" :key="card.id" v-bind="card" >
    <el-card shadow="hover">
       <div class="card-image">
          <img :src="card.src[0]">
      </div>
      <div class="card-content">
        <div class="text-truncate">{{ card.title }}</div>
        <div>{{ card.price }}€ </div>
        <div>{{ card.type }} </div>
        <div class="text-truncate"><i class="el-icon-location-outline"></i> {{ card.location }}</div>
      </div>
    </el-card>
  </el-col>
</el-row>
</template>

<script>

  const cardOptions = [
        {
        title: "Ceci est une plante verte",
        description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        src: ["https://images.unsplash.com/photo-1597055181300-e3633a917c9c?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1064&q=80" , " p" , "p"],
        type: "Ficus",
        size: "Moyenne",
        location: "Montreuil",
        price: 10
        },
        {
        title: "Vend petit bambou",
        description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        src: ["https://images.unsplash.com/photo-1567331711402-509c12c41959?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1073&q=80" , "p" , "p"],
        type: "Bambou",
        size: "Grande",
        location: "Noisy-le-Sec",
        price: 5
        },
        {
        title: "Calathea Medaillon",
        description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        src: ["https://images.unsplash.com/photo-1602879952653-a3830f12a7cb?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=774&q=80" , "p" , "p"],
        type: "Calathea",
        size: "Moyenne",
        location: "Noisy-le-Sec",
        price: 15
        },
        {
        title: "Audrey Ficus à vendre",
        description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        src: ["https://images.unsplash.com/photo-1591656884447-8562e2373a66?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=774&q=80" , "p" , "p"],
        type: "Ficus",
        size: "Moyenne",
        location: "Noisy-le-Grand",
        price: 15
        },
        {
        title: "De l'Aloe Vera pour une peau douce",
        description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        src: ["https://images.unsplash.com/photo-1596547609652-9cf5d8d76921?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1064&q=80" , "p" , "p"],
        type: "Aloe Vera",
        size: "Moyenne",
        location: "Neuilly-sur-Marne",
        price: 15
        },
        {
        title: "Calathea Obifolia",
        description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        src: ["https://images.unsplash.com/photo-1606146350176-804f4c84fb30?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1626&q=80" , "p" , "p"],
        type: "Calathea",
        size: "Grande",
        location: "Neuilly-Plaisance",
        price: 15
        }]

  export default {
    data() {
      return {
        cardOp: cardOptions
      };
    }
  };
</script>