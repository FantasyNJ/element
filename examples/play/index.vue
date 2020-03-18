<template>
  <div style="margin: 20px;">
    <el-time-picker
      is-range
      v-model="value1"
      format="HH:mm"
      value-format="HH:mm"
      :editable="false"
      range-separator="至"
      start-placeholder="开始时间"
      end-placeholder="结束时间"
      placeholder="选择时间范围"
      :picker-options="{
        selectableRange: '04:00:00 - 23:00:00'
      }"
      :isCrossDays="true"
      :clearable="false"
    >
    </el-time-picker>
    <el-time-picker
      is-range
      v-model="value2"
      format="HH:mm"
      value-format="HH:mm"
      :editable="false"
      range-separator="至"
      start-placeholder="开始时间"
      end-placeholder="结束时间"
      placeholder="选择时间范围">
    </el-time-picker>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        value1: ['08:40', '09:40'],
        value2: ['08:40', '09:40']
      };
    }
  };
</script>
