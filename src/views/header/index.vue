<template>
  <div>
    <div class="header_title">
      <img
        src="https://sf6-scmcdn2-tos.pstatp.com/xitu_juejin_web/img/logo.a7995ad.svg"
        alt=""
        class="logo"
      />
      <div class="header_content">
        <div class="header_content_title" v-for="(item, index) in titleList" :key="index">
          {{ item.title }}
        </div>
      <div><img style="width:100px" src="https://sf6-scmcdn2-tos.pstatp.com/xitu_juejin_web/img/2020.933bf44.svg" alt=""></div>
      </div>

      <div class="input_border">
        <input type="text" class="search" />
      </div>
      <div>
        <button class="button_base">写文章</button>
      </div>
      <div>
        <button class="button_base">登陆</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      titleList: [
        {
          title: "首页",
          listsecond: ["推荐", "后端", "前端", "Android", "ios"],
        },
        {
          title: "沸点",
          listsecond: [
            "上班摸鱼",
            "内推招聘",
            "今天学到了",
            "每日算法题",
            "更多话题+",
          ],
        },
        {
          title: "小册",
          listsecond: ["开发工具", "代码人生", "阅读"],
        },
        {
          title: "活动",
          listsecond: ["掘金相亲", "掘金交友"],
        },
      ],
    };
  },
};
</script>

// <style lang="scss" scoped>
.logo{
    padding: 0 10px 0 18px;
}
.header_title {
  width: 1000px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  height:60px;
  .header_content{
      flex: 1;
      display: flex;
    //   justify-content: space-around;
      .header_content_title{
          width: 67px;
          text-align: center;
      }
  }

.input_border{
    padding: 0 14px;
    width: 188px;
    background: red;
    display: flex;
    justify-content: flex-end;
      .search{
      width: 162px;
      height: 15px;
      padding: 4px;
  }

}
.button_base{
    width: 80px;
    // height: 60px;
    height: 24px;
    margin: 0 7px 0 7px;
    
}

}
</style>