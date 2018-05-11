<template>
  <div class="hello">
       <span>添加大款用途</span>
       <dms-select
       placeholder='请输入打款用途并查询'
       :optionsList='lists'
       optionTitle='打款用途'
       @checkedMessage='showMesage'
       multiple
       ></dms-select>
       <br>
       <span ></span>
  </div>
</template>

<script>
import dmsSelect from './dmsSelect'
export default {
  name: 'HelloWorld',
  data () {
    return {
      lists:[
        {key:1,title:'整车采购'},
        {key:2,title:'保证金'},
        {key:3,title:'批量采购'},
        {key:4,title:'购车金'},
        {key:5,title:'押金'},
        {key:6,title:'维修金'},
        {key:7,title:'维修单'},
        {key:8,title:'故障单'},
        {key:9,title:'备购'},
        {key:10,title:'采购'},
        {key:11,title:'采购'},
        {key:12,title:'采购'},
        {key:13,title:'采购'},
        {key:14,title:'采购'},
        {key:15,title:'采购'},
        {key:16,title:'件采购'},
        {key:17,title:'件采购'},
        {key:18,title:'件采购'},
        {key:19,title:'件采购'},
        {key:20,title:'件采购'},
        {key:21,title:'件采购'},
        {key:22,title:'件采购'},
        {key:23,title:'件采购'},
        {key:24,title:'件采购'},
        {key:25,title:'件采购'},
        {key:26,title:'件采购'},
        {key:27,title:'备件采购'},
        {key:28,title:'件采购'},
      ]
    }
  },
  components:{
    dmsSelect
  },
  methods:{
    showMesage(data){
      console.log('收到信息',data);
    }
  }
}
</script>



