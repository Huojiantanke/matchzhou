<template>
  <div>
    <van-cell is-link @click="showPopup">登录/注册</van-cell>
    <van-popup v-model="show" round position="bottom" :style="{ height: '50%' }">
      <div class="box">
          <div class="doLogin">
            <div>
              <span style="font-weight: bolder;">账号登录</span>
              <span>短信登录</span>
            </div>
          </div>
      </div>
    </van-popup>
  </div>
</template>

<script>
  export default {
  data() {
    return {
      show: false,
    };
  },

  methods: {
    showPopup() {
      this.show = true;
    },
  },
};
</script>

<style lang="scss" scoped>
  .box{
    text-align: left;
    padding: 4vw;
    .doLogin{
      padding:5px 10px;
    // font-weight: bolder;
  }
  }
  
</style>