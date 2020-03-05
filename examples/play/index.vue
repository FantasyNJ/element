<template>
  <div style="margin: 20px;">
    <el-time-picker
      is-range
      v-model="value1"
      value-format="HH:mm"
      format="HH:mm"
      :picker-options="{
        selectableRange: '04:00:00 - 23:59:00'
      }"
      placeholder="选择时间范围"
      @change="change"
    >
    </el-time-picker>
    <br>
    <el-time-picker
      v-model="value2"
      :picker-options="{
        selectableRange: '18:30:00 - 20:30:00'
      }"
      value-format="HH:mm"
      format="HH:mm"
      placeholder="任意时间点">
    </el-time-picker>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        value1: ['08:40', '07:40'],
        value2: '08:40'
      };
    },
    methods: {
      change(val){
        console.log(val)
      }
    }
  };
</script>
