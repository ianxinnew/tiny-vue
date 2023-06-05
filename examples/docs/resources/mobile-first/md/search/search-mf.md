<style scoped>
#ji-ben-yong-fa + div>>>.hae-tabs__content {
  min-height: 150px;
}
#dao-hang-sou-suo + p + div>>>.hae-tabs__content {
  min-height: 150px;
}
</style>
<div class="demo-header">
<p class="overviewicon">
  <span class="wapi-form-search"/>
</p>
 
## Search 搜索
 
<nova-uxlink widget-name="Search"></nova-uxlink>
 
指定条件对象进行搜索数据。
</div>
 
### 基本用法
 
<nova-demo-view link="search/basic-usage.vue"></nova-demo-view>
 
### 回车搜索
 
可通过 `is-enter-search` 属性设置按回车键后触发搜索。
 
<nova-demo-view link="search/enter-search.vue"></nova-demo-view>
 
### 自定义 search 事件
 
<nova-demo-view link="search/search-events.vue"></nova-demo-view>
 
### 自定义 change 事件
 
<nova-demo-view link="search/change-events.vue"></nova-demo-view>
 
<br />
 
### 按钮搜索
 
可通过 `show-button` 属性对移动端设置按钮搜索。
 
<nova-demo-view link="search/button-search.vue"></nova-demo-view>
 
<br />