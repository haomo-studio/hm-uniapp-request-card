<template>
  <div class="hm-request-card">
    <div class="box">
      <div class="head">
        <div class="outer">
          <image class="avator" :src="options.avator" />
          <div class="wrap">
            <text class="name">{{ options.name }}</text>
            <text class="address">{{ options.address }}</text>
          </div>
        </div>
        <image class="statimg" :src="options.statimg" />
      </div>
      <div class="body">
        <div class="block">
          <image class="largeIcon" :src="options.largeIcon" />
          <text class="agree">{{ options.agree }}</text>
        </div>
        <div class="tagWrap">
          <text class="cancel">{{ options.cancel }}</text>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmRequestCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-request-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          avator:
            '/static/hm-request-card/images/img_25260_0_0.png',
          name: '马莉',
          address: '上海',
          statimg:
            '/static/hm-request-card/images/img_25260_0_1.png',
          largeIcon:
            '/static/hm-request-card/images/img_25260_0_2.png',
          agree: '同意',
          cancel: '取消'
        };
      }
    }
  },
  data() {
    return {};
  },
  methods: {}
};
</script>
<style>
@import './index.response.css';
</style>
