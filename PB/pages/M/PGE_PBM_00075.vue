<template>
  <sui-page class="custom_page">
    <sui-page-header2 :page-id="this.$options.name" />
    <sui-page-contents>
      <div class="comm_title_wrap">
        <h4>스케줄러 정보</h4>
      </div>
      <ur-form-box toggleable>
        <ur-form-item
          class="flex_wrap"
          label="스케줄명"
          :label-align="'right'"
          required
          style="width: 50%; height: auto"
        >
          <ur-text-field style="width: 100%" value="" />
        </ur-form-item>
        <ur-form-item
          class="flex_wrap"
          label="설명"
          :label-align="'right'"
          required
          style="width: 50%; height: auto"
        >
          <ur-text-field style="width: 100%" value="" />
        </ur-form-item>
        <ur-form-item
          class="flex_wrap"
          label="Cron EXP"
          :label-align="'right'"
          required
          style="width: 50%; height: auto"
        >
          <ur-text-field style="width: 100%" value="" />
        </ur-form-item>
        <ur-form-item
          class="flex_wrap"
          label="사용 여부"
          :label-align="'right'"
          required
          style="width: 50%; height: auto"
        >
          <div class="radioForm">
            <ur-radio v-model="v1" value="Radio 00075_01" sm>Y</ur-radio>
            <ur-radio v-model="v1" value="Radio 00075_02" sm>N</ur-radio>
          </div>
          <!-- <ur-radio-wrapper v-model="valueR1" :items="itemsR1" sm /> -->
        </ur-form-item>
        <ur-form-item
          class="flex_wrap"
          label="Trigger Name"
          :label-align="'right'"
          required
          style="width: 50%; height: auto"
        >
          <ur-text-field style="width: 100%" value="" />
        </ur-form-item>
        <ur-form-item
          class="flex_wrap"
          label="Trigger Group"
          :label-align="'right'"
          required
          style="width: 50%; height: auto"
        >
          <ur-text-field style="width: 100%" value="" />
        </ur-form-item>
        <ur-form-item
          class="flex_wrap"
          label="Job Name"
          :label-align="'right'"
          required
          style="width: 50%; height: auto"
        >
          <ur-text-field style="width: 100%" value="" />
        </ur-form-item>
        <ur-form-item
          class="flex_wrap"
          label="Job Group"
          :label-align="'right'"
          required
          style="width: 50%; height: auto"
        >
          <ur-text-field style="width: 100%" value="" />
        </ur-form-item>
        <ur-form-item
          class="flex_wrap"
          label="Class명"
          :label-align="'right'"
          required
          style="width: 50%; height: auto"
        >
          <ur-text-field style="width: 100%" value="" />
        </ur-form-item>
        <ur-form-item
          class="flex_wrap"
          label="Method명"
          :label-align="'right'"
          required
          style="width: 50%; height: auto"
        >
          <ur-text-field style="width: 100%" value="" />
        </ur-form-item>
      </ur-form-box>
      <div class="btn_wrap mt10">
        <div class="right_box">
          <ur-button> 목록 </ur-button>
          <ur-button color="violet"> 저장 </ur-button>
        </div>
      </div>

      <!-- <sui-page-footer class="comm_btn_wrap">
        <div class="btn_wrap">
          <div class="left_box">
            <ur-button> 목록 </ur-button>
          </div>
          <div class="right_box">
            <ur-button color="violet"> 저장 </ur-button>
          </div>
        </div>
      </sui-page-footer> -->
    </sui-page-contents>
  </sui-page>
</template>
<script>
export default {
  name: "PGE_PBM_00075", // eslint-disable-line vue/name-property-casing
  components: {},
  data() {
    return {
      // 라디오 버튼
      v1: "Radio 00075_01",

      valueR1: "1",
    };
  },
  computed: {
    // 계산된 속성, date pickproperty로 사용가능
    itemsR1() {
      const rtn = [];
      rtn.push({ value: "1", text: "Y" });
      rtn.push({ value: "2", text: "N" });
      return rtn;
    },
  },
  watch: {
    // data 변경시 특정 함수를 호출 해야 하는 경우(async 등)
  },
  created() {},
  mounted() {},
  methods: {},
};
</script>
<style scoped></style>
