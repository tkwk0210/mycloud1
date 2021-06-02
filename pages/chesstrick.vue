<template>
  <div>
    <section class="hero is-primary">
      <div class="hero-body">
          <p class="title"><i class="fas fa-chess"></i>
           Chess Game
          </p>
          <p class="subtitle">
            체스 특수 행마법
          </p>
      </div>
    </section>
    <section class="notification is-warning">
        <table class="table is-hoverable">
            <thead>
                <th>특수 행마법</th>
                <tr>
                    <th>이름</th>
                    <th>조건</th>
                    <th>방법</th>
                </tr>
            </thead>
            <tbody >
                <tr v-for="trickname in tablechesstrick" :key="trickname">
                    <td >
                        <tr>{{trickname}}</tr>
                    </td>
                </tr>
                <tr>
                    <td></td>
                </tr>

            </tbody>
        </table>
    </section>
    </div>
</template>
<script>
import chesstrick from "~/assets/chesstrick.json"
export default {
    data() {
        return {
            tablechesstrick: chesstrick.system_names,
            tablechesstrickway: chesstrick.way
        }
    }
};
</script>