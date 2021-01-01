<template>
  <v-container class="grey lighten-5" style="text-align: center; font-size: 30px">
    <v-row
      no-gutters
      >
      <v-col
        v-for="f in firstLine"
        :key="f"
        >
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <p>{{ f }}</p>
        </v-card>
      </v-col>
    </v-row>
    <!-- first line -->
    <v-row
      no-gutters
      >
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          p1
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75">-</v-card>
      </v-col>
      <!-- testarea -->
      <v-col
        >
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p1p2"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <v-col
        >
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p1p3"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <v-col
        >
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p1p4"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <!-- mutch point -->
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p1winround }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p1loseround }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p1diff }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p1win }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p1rank }}
        </v-card>
      </v-col>
    </v-row>

    <!-- second line -->
    <v-row
      no-gutters
      >
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          p2
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p2p1"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75">-</v-card>
      </v-col>
      <!-- testarea -->
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p2p3"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p2p4"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <!-- mutch point -->
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p2winround }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p2loseround }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p2diff }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p2win }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p2rank }}
        </v-card>
      </v-col>
    </v-row>

    <!-- therd line -->
    <v-row
      no-gutters
      >
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          p3
        </v-card>
      </v-col>
      <!-- testarea -->
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p3p1"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p3p2"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75">-</v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p3p4"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <!-- mutch point -->
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p3winround }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p3loseround }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p3diff }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p3win }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p3rank }}
        </v-card>
      </v-col>
    </v-row>

    <!-- forth line -->
    <v-row
      no-gutters
      >
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          p4
        </v-card>
      </v-col>
      <!-- testarea -->
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p4p1"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p4p2"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          <v-textarea
            outlined
            rows="1"
            v-model="p4p3"
          >
          </v-textarea>
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75">-</v-card>
      </v-col>
      <!-- mutch point -->
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p4winround }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p4loseround }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p4diff }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p4win }}
        </v-card>
      </v-col>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
          height="75"
          >
          {{ p4rank }}
        </v-card>
      </v-col>
    </v-row>
    <v-btn @click=update>update</v-btn>
    <v-btn @click=ranking>ranking</v-btn>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      firstLine: ["name", "p1", "p2", "p3", "p4", "WR", "LR", "diff", "勝数", "順位"],
      p1p2: "",
      p1p3: "",
      p1p4: "",
      p1winround: 0,
      p1loseround: 0,
      p1diff: 0,
      p1win: 0,
      p1rank: 0,
      p2p1: "",
      p2p3: "",
      p2p4: "",
      p2winround: 0,
      p2loseround: 0,
      p2diff: 0,
      p2win: 0,
      p2rank: 0,
      p3p1: "",
      p3p2: "",
      p3p4: "",
      p3winround: 0,
      p3loseround: 0,
      p3diff: 0,
      p3win: 0,
      p3rank: 0,
      p4p1: "",
      p4p2: "",
      p4p3: "",
      p4winround: 0,
      p4loseround: 0,
      p4diff: 0,
      p4win: 0,
      p4rank: 0,
    }
  },
  mounted() {
  },
  methods: {
    update() {
      // 2先
      if (this.p1p2.match(/\n/) || this.p1p3.match(/\n/) || this.p1p4.match(/\n/) ||
      this.p2p1.match(/\n/) || this.p2p3.match(/\n/) || this.p2p4.match(/\n/) || 
      this.p3p1.match(/\n/) || this.p3p1.match(/\n/) || this.p3p4.match(/\n/) ||
      this.p4p1.match(/\n/) || this.p4p2.match(/\n/) || this.p4p3.match(/\n/)
      ) {
        const p1p2 = this.p1p2.split("\n");
        const p1p3 = this.p1p3.split("\n");
        const p1p4 = this.p1p4.split("\n");
        const p1winLose = [p1p2, p1p3, p1p4];
        let p1winround = 0;
        let p1loseround = 0;
        let p1win = 0;
        p1winLose.forEach((twoFTResult) => {
          // 1戦の結果
          twoFTResult.forEach((oneRResult) => {
          const result = this.updateButtle(oneRResult);
          p1winround += result.winround;
          p1loseround += result.loseround;
          p1win += result.win;
          })
        }) 
        this.updateResult("p1", p1winround, p1loseround, p1win);

        const p2p1 = this.p2p1.split("\n");
        const p2p3 = this.p2p3.split("\n");
        const p2p4 = this.p2p4.split("\n");
        const p2winLose = [p2p1, p2p3, p2p4];
        let p2winround = 0;
        let p2loseround = 0;
        let p2win = 0;
        p2winLose.forEach((twoFTResult) => {
          // 1戦の結果
          twoFTResult.forEach((oneRResult) => {
          const result = this.updateButtle(oneRResult);
          p2winround += result.winround;
          p2loseround += result.loseround;
          p2win += result.win;
          })
        }) 
        this.updateResult("p2", p2winround, p2loseround, p2win)

        const p3p1 = this.p3p1.split("\n");
        const p3p2 = this.p3p2.split("\n");
        const p3p4 = this.p3p4.split("\n");
        const p3winLose = [p3p1, p3p2, p3p4];
        let p3winround = 0;
        let p3loseround = 0;
        let p3win = 0;
        p3winLose.forEach((twoFTResult) => {
          // 1戦の結果
          twoFTResult.forEach((oneRResult) => {
          const result = this.updateButtle(oneRResult);
          p3winround += result.winround;
          p3loseround += result.loseround;
          p3win += result.win;
          })
        }) 
        this.updateResult("p3", p3winround, p3loseround, p3win)

        const p4p1 = this.p4p1.split("\n");
        const p4p2 = this.p4p2.split("\n");
        const p4p3 = this.p4p3.split("\n");
        const p4winLose = [p4p1, p4p2, p4p3];
        let p4winround = 0;
        let p4loseround = 0;
        let p4win = 0;
        p4winLose.forEach((twoFTResult) => {
          // 1戦の結果
          twoFTResult.forEach((oneRResult) => {
          const result = this.updateButtle(oneRResult)
          p4winround += result.winround;
          p4loseround += result.loseround;
          p4win += result.win;
          })
        }) 
        this.updateResult("p4", p4winround, p4loseround, p4win);

      } else {
      // 1先
      const p1winLose = [this.p1p2, this.p1p3, this.p1p4];
      let p1winround = 0;
      let p1loseround = 0;
      let p1win = 0;
      p1winLose.forEach((oneRResult) => {
          const result = this.updateButtle(oneRResult)
          p1winround += result.winround;
          p1loseround += result.loseround;
          p1win += result.win;
      })
      this.updateResult("p1", p1winround, p1loseround, p1win)

      const p2winLose = [this.p2p1, this.p2p3, this.p2p4];
      let p2winround = 0;
      let p2loseround = 0;
      let p2win = 0;
      p2winLose.forEach((oneRResult) => {
          const result = this.updateButtle(oneRResult)
          p2winround += result.winround;
          p2loseround += result.loseround;
          p2win += result.win;
      })
      this.updateResult("p2", p2winround, p2loseround, p2win)

      const p3winLose = [this.p3p1, this.p3p2, this.p3p4];
      let p3winround = 0;
      let p3loseround = 0;
      let p3win = 0;
      p3winLose.forEach((oneRResult) => {
          const result = this.updateButtle(oneRResult)
          p3winround += result.winround;
          p3loseround += result.loseround;
          p3win += result.win;
      })
      this.updateResult("p3", p3winround, p3loseround, p3win)

      const p4winLose = [this.p4p1, this.p4p2, this.p4p3];
      let p4winround = 0;
      let p4loseround = 0;
      let p4win = 0;
      p4winLose.forEach((oneRResult) => {
          const result = this.updateButtle(oneRResult)
          p4winround += result.winround;
          p4loseround += result.loseround;
          p4win += result.win;
      })
      this.updateResult("p4", p4winround, p4loseround, p4win)
      }
    },
    ranking() {
      try{
      const rank =  {"p1": this.p1win, "p2": this.p2win, "p3": this.p3win, "p4": this.p4win}
      const values = Object.entries(rank);
      values.sort(function(p1, p2){
        const p1Val = p1[1], p2Val = p2[1];
        return p2Val - p1Val;
      })
      let sameWin = 0;
      let sameWinIndex = [];
      // 同じ勝数のインデックスを調べる
      values.forEach((v, i) => {
        if (i === 0) {
          sameWin = v[1];
          return;
        }
        if (v[1] === sameWin && v[1] !== 0) {
          if (i === 1) {
          sameWinIndex.push(i-1);
          sameWinIndex.push(i);
          } else {
            sameWinIndex.push(i);
          }
        } else {
          sameWin = v[1];
        }
      })

      const diffs = {
        "p1": this.p1diff,
        "p2": this.p2diff,
        "p3": this.p3diff,
        "p4": this.p4diff
      }
      let sameWinPlayer = {};
      // 同じ勝数のプレイヤー: diffを作る
      sameWinIndex.forEach((i) => {
        sameWinPlayer[values[i][0]] = diffs[values[i][0]];
      }) 

      const sortPlayer = Object.entries(sameWinPlayer);
      sortPlayer.sort(function(p1, p2){
        const p1Val = p1[1], p2Val = p2[1];
        return p2Val - p1Val;
      })
       
      sameWinIndex.forEach((v,i) => {
        values[v] = sortPlayer[i];
      })
      values.forEach((v,i) => {
        values[i][1] = i+1
      })

      const ranking = Object.fromEntries(values);
      this.p1rank = ranking.p1;
      this.p2rank = ranking.p2;
      this.p3rank = ranking.p3;
      this.p4rank = ranking.p4;
      } catch(err) {
        alert("判定出来ませんでした")
      } 
    },
    updateButtle(oneRResult) {
      const winLose = oneRResult.split("-");
      let winround = 0;
      let loseround = 0;
      let win = 0;

      if (winLose.length === 2) {
        let winr = 0;
        let loser = 0;
        winLose.forEach((v, i) => {
          if (i === 0) {
            winr = Number(v);
            winround += Number(v);
          } else if (i === 1) {
            loser = Number(v);
            loseround += Number(v);
          }
        })
        if (winr > loser) {
          win += 1;
        }
      }
      const result = {
        "winround": winround,
        "loseround": loseround,
        "win": win
      }
      return result
    },
    updateResult(player, winround, loseround, win) {
        switch (player) {
          case "p1":
            this.p1winround = winround;
            this.p1loseround = loseround;
            this.p1win = win;
            this.p1diff = winround - loseround;
          break;
          case "p2":
            this.p2winround = winround;
            this.p2loseround = loseround;
            this.p2win = win;
            this.p2diff = winround - loseround;
          break;
          case "p3":
            this.p3winround = winround;
            this.p3loseround = loseround;
            this.p3win = win;
            this.p3diff = winround - loseround;
          break;
          case "p4":
            this.p4winround = winround;
            this.p4loseround = loseround;
            this.p4win = win;
            this.p4diff = winround - loseround;
          break;
          default:
        }
    }
  }
}
</script>

<style>
</style>
