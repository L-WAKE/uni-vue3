<template>
  <view class="content">
    <image class="logo" src="/static/logo.png"></image>
    <view class="text-area">
      <text class="title">{{ title }}</text>
    </view>
    <view style="padding: 20px">
      <uv-button>默认按钮</uv-button>
      <uv-button type="primary">主要按钮</uv-button>
      <uv-button type="success">成功按钮</uv-button>
      <uv-button type="info">信息按钮</uv-button>
      <uv-button type="warning">警告按钮</uv-button>
      <uv-button type="error">危险按钮</uv-button>
    </view>
  </view>
  <view style="padding: 20px"> </view>
</template>

<script>
export default {
  data() {
    return {
      title: "Hello",
    };
  },
  onLoad() {},
  methods: {},
};
</script>

<style>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.logo {
  height: 200rpx;
  width: 200rpx;
  margin-top: 200rpx;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 50rpx;
}

.text-area {
  display: flex;
  justify-content: center;
}

.title {
  font-size: 36rpx;
  color: #8f8f94;
}
</style>
