<template>
    <el-popover
      placement="bottom"
      trigger="click"
      >
        <el-select
            v-model="value"
            multiple
            filterable
            remote
            reserve-keyword
            placeholder="Entrez un mot-clé"
            >
            <el-option
              v-for="item in states"
              :key="item.name"
              :value="item.name">
              {{item.name}}
            </el-option>
          </el-select>
      <el-button slot="reference">Ville</el-button>
    </el-popover>
</template>

<script>
   export default {
    data() {
      return {
        options: [],
        value: [],
        list: [],
        loading: false,
        states: [
          {
            id: 35352,
            department_code: "93",
            insee_code: "93048",
            zip_code: "93100",
            name: "Montreuil",
            slug: "montreuil",
            gps_lat: 48.86430191489363,
            gps_lng: 2.45081031914894
          },
          {
            id: 35353,
            department_code: "93",
            insee_code: "93049",
            zip_code: "93360",
            name: "Neuilly-Plaisance",
            slug: "neuilly plaisance",
            gps_lat: 48.86486195121952,
            gps_lng: 2.5127263414634102
          },
          {
            id: 35354,
            department_code: "93",
            insee_code: "93050",
            zip_code: "93330",
            name: "Neuilly-sur-Marne",
            slug: "neuilly sur marne",
            gps_lat: 48.86526206896551,
            gps_lng: 2.5367218390804602
          },
          {
            id: 35355,
            department_code: "93",
            insee_code: "93051",
            zip_code: "93160",
            name: "Noisy-le-Grand",
            slug: "noisy le grand",
            gps_lat: 48.83600000000001,
            gps_lng: 2.56563018348624
          },
          {
            id: 35356,
            department_code: "93",
            insee_code: "93053",
            zip_code: "93130",
            name: "Noisy-le-Sec",
            slug: "noisy le sec",
            gps_lat: 48.88746432098765,
            gps_lng: 2.45495283950617
          }
        ]
      }
    },
    // mounted() {
    //   this.list = this.states.map( item => {
    //     return { value: `value:${item}`, label: `label:${item}` };
    //   });
    //   console.log(this.list)
    //   console.log(this.states.name)
    // },
    // methods: {
    //   remoteMethod(query) {
    //     if (query !== '') {
    //       this.loading = true;
    //       setTimeout(() => {
    //         this.loading = false;
    //         this.options = this.list.filter(item => {
    //           return item.label.toLowerCase()
    //             .indexOf(query.toLowerCase()) > -1;
    //         });
    //       }, 200);
    //     } else {
    //       this.options = [];
          
    //     }console.log(this.options)
    //   }
    // }
  }
</script>