<template>
    <div class="m_skill_item">
        <div >{{ title }}</div>
        <div class="m_skill_item_progress" >
            <div class="progress" :style="{ width: progress+'%'}" >
                <span class="number">{{ progress }}%</span> 
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'SkillItem',
  data: () => {
      return {
          test: null
      }
  },
  props: {
      progress: {
        type: Number,
        required: true
      },
      title : {
          type: String,
          required: false
      }
  },
  mounted () {
      console.log(this.progress);
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.m_skill_item {
  font-size: 16px;
  text-transform: uppercase;
  font-family: "Raleway-Bold";
  color: #333333;
  margin-top: 15px;
  .m_skill_item_progress {
    height: 30px;
    background-color: #dcdcdc;
    width: 100%;
    .progress {
      height: 100%;
      background-color: var(--warning-color);
      display: flex;
      padding-right: 10px;
      .number{
        align-self: center;
        margin-left: auto;
        color: white;
      }
    }
    
  }
}
</style>
