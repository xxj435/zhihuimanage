<template>
  <div class="home">
    <el-container>
      <el-header>
        <Header />
      </el-header>
      <el-main>
        <div class="content">
          <div class="left_content">
            <div class="manage">
              <h2>智慧园区</h2>
              <h2>数字化管理</h2>
              <div class="text">为园区提供数字化管理解决方案实现智慧园区原理</div>
              <el-input
                placeholder="请输入手机号立即开始"
                v-model="input2"
              >
                <el-button
                  slot="append"
                  type="primary"
                >免费使用</el-button>
              </el-input>
            </div>
          </div>
          <div class="right_content">
            <img
              src="../assets/logo.jpg"
              alt=""
            >
            <p>　　技术云平台优势是汇聚长三角多低协会和联盟的专家库资源, 为企业精准匹配知识产权服务领域的专家资源, 小到商标注册, 大到专利保护, 技术云平台只推送大专家服务, 因为知识产权是企业的生命. 从诞生之日起, 技术云为你配备行业内的权威专家, 护航企业发展!</p>
          </div>
        </div>

      </el-main>
    </el-container>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
export default {
  name: "Home",
  components: {
    Header,
  },
};
</script>
<style lang="scss" scoped>
.home {
  .content {
    display: flex;
    justify-content: space-around;
    .left_content {
      width: 300px;
      .manage {
        h2 {
          font-size: 40px;
        }
        .text {
          font-size: 15px;
        }
        .el-input.el-input-group.el-input-group--append {
          font-size: 12px;
          margin-top: 30px;
        }
      }
    }
    .right_content {
      display: flex;
      flex-direction: column;
      align-items: center;
      width: 800px;
      p {
        font-size: 14px;
        font-weight: 500;
      }
    }
  }
}
</style>
