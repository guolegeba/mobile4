<template>
  <div>
    <h3>xixi</h3>
    <van-button type="primary">按钮</van-button>
    <van-address-edit
        :area-list="areaList"
        show-postal
        show-delete
        show-set-default
        show-search-result
        :search-result="searchResult"
        :area-columns-placeholder="['请选择', '请选择', '请选择']"
        @save="onSave"
        @delete="onDelete"
        @change-detail="onChangeDetail"
    />
    
  </div>
</template>

<script>
import { Toast } from 'vant';
import areaData from '../utils/areaData';

export default {
  data() {
    return {
      areaList:areaData,
      searchResult: [],
    }
  },
  methods: {
    onSave() {
      Toast('save');
    },
    onDelete() {
      Toast('delete');
    },
    onChangeDetail(val) {
      if (val) {
        this.searchResult = [
          {
            name: '黄龙万科中心',
            address: '杭州市西湖区',
          },
        ]
      } else {
        this.searchResult = [];
      }
    },
  },
};
</script>

<style>

</style>