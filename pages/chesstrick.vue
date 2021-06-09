<template>
  <div>
    <section class="hero is-primary">
      <div class="hero-body">
          <p class="title"><i class="fas fa-chess"></i>
           체스 특수 행마법
          </p>
          <p class="subtitle">
            특수 행마법에 대해 알아보자.
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
                    <td>
                        {{trickname}}
                    </td>
                    <td>
                        <div v-if="trickname[0] =='캐'">
                            1. 킹과 캐슬링을 하려는 룩 사이를 비워 둬야 한다.
                            <br>2. 캐슬링을 하려는 룩과 킹은 한 번도 이동한 적이 없어야 한다. 이동 후 다시 원래 자리로 돌아오는 것도 안 된다.
                            <br>3. 두 룩 중 한 쪽만 이동한 적이 있으면 이동한 적이 없는 룩 쪽으로만 캐슬링을 할 수 있다.
                            <br>4. 킹이 총 세 위치에서 체크 상태가 아니어야 한다: 원래 위치, 캐슬링 방향으로 한 칸 옆 위치(거쳐가야 할 칸), 두 칸 옆 위치(목적지). 룩은 이러한 제약 조건이 없다.
                        </div>
                        <div v-if="trickname[0] =='승'">
                            폰이 상대방 진영 끝 랭크까지 갔을때
                        </div>
                        
                        <div v-if="trickname[0] =='앙'">
                            1. 상대방의 폰이 첫 이동으로 2칸을 전진했는데 그 바로 옆 칸에 자신의 폰이 있을 경우
                            <br>2. 상대가 폰을 2칸 움직인 직후에만 행하는 것이 가능하며, 차례를 1번 거른 후에는 앙파상으로 잡을 수 없다.
                        </div>
                        </td>
                    <td>
                        <div v-if="trickname[0] =='캐'" >
                            조건을 충족하는 경우에 킹과 룩을 한 번에 동시에 움직여 각각의 위치를 바꿀 수 있다.
                        </div>
                        <div v-if="trickname[0] =='승'" >
                            폰이 상대편 진영 끝까지 전진했을 경우 그 폰은 폰과 킹을 제외한 다른 모든 기물들 중 하나로 승격할 수 있다
                        </div>
                        <div v-if="trickname[0] =='앙'" >
                            1칸만 이동한 것으로 간주하고 그대로 상대방의 폰을 잡을 수 있으며, 잡은 후에는 반드시 대각선으로 이동해야 한다.
                        </div>
                    </td>
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
        }
    }
};
</script>