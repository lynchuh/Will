<template>
<div style="margin-top:26px">
  <h3>1. 基础用法</h3>
  <div class="demo">
    <w-tabs selected="first-tab"  style="margin-top:20px;">
      <w-tabs-head>
        <w-tabs-item label="first-tab">Tab 1</w-tabs-item>
        <w-tabs-item label="2">Tab 2</w-tabs-item>
        <w-tabs-item label="third-tab">Tab 3</w-tabs-item>
      </w-tabs-head>
      <w-tabs-body>
        <w-tabs-pane name="first-tab">content of Tab 1</w-tabs-pane>
        <w-tabs-pane name="2">content of Tab 2</w-tabs-pane>
        <w-tabs-pane name="third-tab">content of Tab 3</w-tabs-pane>
      </w-tabs-body>
    </w-tabs>
  </div>  
</div>
</template>
<script>
import Tabs from '../../../src/tabs'
import TabsHead from '../../../src/tabs-head'
import TabsBody from '../../../src/tabs-body'
import TabsItem from '../../../src/tabs-item'
import TabsPane from '../../../src/tabs-pane'

export default {
  components:{
    'w-tabs':Tabs,
    'w-tabs-head':TabsHead,
    'w-tabs-item':TabsItem,
    'w-tabs-body':TabsBody,
    'w-tabs-pane':TabsPane,
  }
};
</script>
<style lang="scss" scoped>
.demo{
  box-shadow: 0 0 46px 0px rgba(0, 0, 0, 0.1);
  padding: 22px;
  padding-top: 1px;
  border-radius: 6px;
}
</style>


