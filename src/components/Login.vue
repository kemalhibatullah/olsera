<template>
  <div
    id="div1"
    style="
      height: 100vh;
      width: 100wh;
      display: flex;
      justify-content: center;
      align-items: center;
    "
  >
    <div style="min-width: 300px">
      <el-card class="box-card">
        <div class="text item" style="margin-bottom: 30px">Login</div>
        <el-row style="margin-bottom: 30px">
          <el-input
            v-model="username"
            placeholder="Username"
            prefix-icon="el-icon-user"
          />
        </el-row>
        <el-row style="margin-bottom: 30px">
          <el-input
            v-model="password"
            placeholder="Password"
            prefix-icon="el-icon-lock"
            show-password
          />
        </el-row>
        <el-button type="primary">Login</el-button>
      </el-card>
    </div>
  </div>
</template>

<script>
import { defineComponent, ref } from "vue";
export default defineComponent({
  setup() {
    return {
      username: ref(""),
      password: ref(""),
    };
  },
  data(){
       return{
       }
  },
});
</script>

<style scoped>
#div1{
  background-image: linear-gradient(90deg, #00d2ff 0%, #3a47d5 100%);
}
</style>
