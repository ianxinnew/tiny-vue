<template>
  <tiny-milestone :data="milestoneData" :milestones-status="statusMap"></tiny-milestone>
</template>

<script lang="jsx">
import { Milestone } from '@opentiny/vue'

export default {
  components: {
    TinyMilestone: Milestone
  },
  data() {
    return {
      // 里程碑样式
      statusMap: {
        completed: '#5938b9',
        doing: '#7ED321',
        back: '#f5222d',
        end: '#faad14',
        cancel: '#d9d9d9'
      },
      // 数据源
      milestoneData: [
        {
          name: '自定义数据1',
          time: '2018-9-7',
          status: 'completed'
        },
        {
          name: '自定义数据2',
          time: '2018-9-8',
          status: 'completed'
        },
        {
          name: '自定义数据3',
          time: '2018-9-10',
          status: 'doing',
          content: null
        },
        {
          name: '自定义数据4',
          time: '2018-9-9',
          status: 'cancel'
        },
        {
          name: '自定义数据5',
          time: '2018-9-11',
          status: 'back'
        },
        {
          name: '自定义数据6',
          time: '2018-9-9',
          status: 'end'
        }
      ]
    }
  }
}
</script>
