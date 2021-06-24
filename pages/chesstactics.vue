<template>
  <div>
    <section class="hero is-primary">
      <div class="hero-body">
          <p class="title"><i class="fas fa-chess"></i>
           체스 전술
          </p>
          <p class="subtitle">
            체스 전술에 대해 알아보자
          </p>
      </div>
    </section>
        <article class="notification is-warning is-light">
            <div class="notification is-warning is-light-header">
                <th>체스 전술</th>
            </div>
            <div class="notification is-warning is-light-body">
                <table class = "table is-bordered">
                <tbody>
                    <tr v-for="tacticsname in tablechesstactics" :key="tacticsname">
                        <td>
                            {{tacticsname}}
                        </td>
                        <td>
                            <div v-if="tacticsname[0] =='포'">
                                가치가 낮은 한 피스가 가치가 높은 2개 이상의 피스를 동시에 공격하는 경우
                            </div>
                            <div v-if="tacticsname[4] =='택'">
                                폰이 상대방 진영 끝 랭크까지 갔을때
                            </div>
                        
                            <div v-if="tacticsname[0] =='핀'">
                               뒤의 피스 때문에 앞의 피스가 움직일 수 없는 경우
                            </div>

                            <div v-if="tacticsname[0] =='스'">
                               앞의 피스를 움직일 수밖에 없어서 뒤의 피스가 잡히는 경우
                            </div>

                            <div v-if="tacticsname[0] =='블'">
                               단기적으로 나쁜 움직임.
                            </div>

                            <div v-if="tacticsname[4] =='크'">
                               2개 이상의 피스로 한꺼번에 체크를 하는 수. 주로 아래에 언급된 디스커버드 체크를 하는 기물이 동시에 체크를 할 때 발생한다.
                            </div>

                            <div v-if="tacticsname[0] =='피'">
                               끝쪽 폰 3개 중에서 중간 하나만 한 칸을 앞으로 전진시키고 그 자리에 비숍을 놓음으로써아주 긴 대각선을 차지하는 수들의 묶음.
                            </div>

                            <div v-if="tacticsname[0] =='트'">
                               같은 피스 또는 나이트와 비숍 간에 서로 잡고 잡히는 관계.
                            </div>

                            <div v-if="tacticsname[0] =='디'">
                               아군 피스 하나를 움직여 다른 아군 피스의 길을 열어 적 킹을 체크하는 수.
                            </div>
                        </td>
                    </tr>
                </tbody>
                </table>
            </div>
        </article>
  </div>
</template>
<script>
import chesstactics from "~/assets/chesstactics.json"
export default {
    data() {
        return {
            tablechesstactics: chesstactics.tactics,
        }
    }
};
</script>