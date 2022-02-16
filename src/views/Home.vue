<template>
  <div class="home">
    <el-container>
      <el-header class="top">
        <Header />
      </el-header>
      <el-main>
        <section class="content">
          <div class="left_content">
            <div class="manage">
              <h2>智慧园区</h2>
              <h2>数字化管理</h2>
              <div class="text">为园区提供数字化管理解决方案实现智慧园区原理</div>
              <el-input
                placeholder="请输入手机号立即开始"
                v-model="input1"
              >
                <el-button
                  slot="append"
                  type="primary"
                >
                  免费使用
                </el-button>
              </el-input>
            </div>
          </div>
          <div class="right_content">
            <img
              style="margin-bottom:30px;"
              src="../assets/logo.jpg"
              alt=""
            >
            <p>　　技术云平台优势是汇聚长三角多低协会和联盟的专家库资源, 为企业精准匹配知识产权服务领域的专家资源, 小到商标注册, 大到专利保护, 技术云平台只推送大专家服务, 因为知识产权是企业的生命. 从诞生之日起, 技术云为你配备行业内的权威专家, 护航企业发展!</p>
          </div>
        </section>
        <section class="img-content">
          <div class="imgbox">
            <img
              src="../assets/ip.jpg"
              alt=""
            >
            <img
              src="../assets/ren.jpg"
              alt=""
            >
          </div>
          <img
            src="../assets/ipren.jpg"
            alt=""
          >
        </section>
        <section class="enterprise">
          <div class="text">
            <p>注册企业<span>XXX</span>家　　　办公企业<span>XXX</span>家</p>
            <img
              src="../assets/map.jpg"
              alt=""
            >
          </div>
          <div>
            <h2>园区注册企业</h2>
            <h2>自动扫描</h2>

            <p>基于园区四至范围,</p>
            <p>自动识别范围内注册的企业</p>
            <img
              class="img"
              src="../assets/xx.jpg"
              alt=""
            >
          </div>
        </section>
        <section class="qiye">
          <div>
            <h2>企业知识产权数据</h2>
            <h2>实时管理</h2>
            <p>实时掌握园区企业知识产权情况</p>
            <p>按月定期更新</p>
          </div>
          <div><img
              src="../assets/data.jpg"
              alt=""
            >
            <div class="list">
              <div class="listbox">
                <img
                  src="../assets/quan.jpg"
                  alt=""
                >
                <span>专利</span>
              </div>
              <div class="listbox">
                <img
                  src="../assets/quan.jpg"
                  alt=""
                >
                <span>商标</span>
              </div>
              <div class="listbox">
                <img
                  src="../assets/quan.jpg"
                  alt=""
                >
                <span>集成电路</span>
              </div>
              <div class="listbox">
                <img
                  src="../assets/quan.jpg"
                  alt=""
                >
                <span>PCT</span>
              </div>
              <div class="listbox">
                <img
                  src="../assets/quan.jpg"
                  alt=""
                >
                <span>软件著作权</span>
              </div>
              <div class="listbox">
                <img
                  src="../assets/quan.jpg"
                  alt=""
                >
                <span>作品著作权</span>
              </div>
            </div>
          </div>
        </section>
        <section class="changsan">
          <img
            src="../assets/map2.jpg"
            alt=""
          >
          <div class="text">
            <p>长三角<span>一体化</span></p>
            <p>IP大专家<span>服务</span></p>
            <p><span>机构</span>派单机构</p>
            <div style="margin-top: 30px;">长三角知识产权运营联盟</div>
            <div>长三角知识产权发展联盟</div>
            <div>长三角多地知识产权协会联合发起</div>
          </div>

        </section>
        <section class="swiper-ha">
          <div class="swiper-container">
            <div class="swiper-wrapper">
              <div class="swiper-slide"><img
                  src="../assets/data.jpg"
                  alt=""
                ></div>
              <div class="swiper-slide"><img
                  src="../assets/map.jpg"
                  alt=""
                ></div>
              <div class="swiper-slide"><img
                  src="../assets/map2.jpg"
                  alt=""
                ></div>
            </div>
          </div>
          <div class="logolist">
            <img
              src="../assets/1.jpg"
              alt=""
            >
            <img
              src="../assets/2.jpg"
              alt=""
            >
            <img
              src="../assets/3.jpg"
              alt=""
            >
            <img
              style="width: 60px;margin-left: 100px;"
              src="../assets/xx.jpg"
              alt=""
            >
          </div>
          <video
            style="margin-top: 100px"
            src="../assets/WeChat_20220216223710.mp4"
            autoplay
          ></video>
        </section>
        <section class="foot">
          <div class="text">
            <h2>免费使用</h2>
            <h4>技术云智慧园区管理系统</h4>
            <p>让科技助力园区管理， 免费使用</p>
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

        </section>
        <section class="footer">
          <div class="icon">
            <img
              class="icon1"
              src="../assets/logo.jpg"
              alt=""
            >
            <div class="icon2">
              <img
                src="../assets/weix.png"
                alt=""
              >
              <img
                src="../assets/weib.png"
                alt=""
              >
            </div>
          </div>
          <div class="txt">
            <div>
              <p style="margin-bottom: 20px;">@teambition</p>
              <p>关于我们</p>
              <p style="margin-top: 70px;">开发者：上海好打发撒旦发公司</p>
            </div>
            <img
              style="width:60px"
              src="../assets/xx.jpg"
              alt=""
            >
          </div>
        </section>
      </el-main>
    </el-container>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import Swiper from "swiper";
import "swiper/dist/css/swiper.min.css";
export default {
  name: "Home",
  components: {
    Header,
  },
  data() {
    return {
      input1: "",
      input2: "",
    };
  },
  mounted() {
    var mySwiper = new Swiper(".swiper-container", {
      autoplay: 3000, //可选选项，自动滑动
      loop: true,
    });
  },
  methods: {
    goAbout() {
      console.log(11);
      this.$router.push({ path: "/About" });
    },
  },
};
</script>
<style lang="scss" scoped>
.home {
  .el-main {
    padding: 0;
  }
  .content {
    height: 600px;
    display: flex;
    align-items: center;
    justify-content: space-around;
    background-image: linear-gradient(to right, #fff, #f6f6fa);
    .left_content {
      width: 245px;
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
      width: 565px;
      p {
        font-size: 14px;
        font-weight: 500;
      }
    }
  }
  .img-content {
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 600px;
    box-shadow: 0 2px 12px 0 rgb(0 0 0 / 10%);
    .imgbox {
      display: flex;
      flex-direction: column;
    }
  }
  .enterprise {
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 600px;
    position: relative;
    box-shadow: 0 2px 12px 0 rgb(0 0 0 / 10%);
    .text {
      font-size: 20px;
      font-weight: 600;
      p {
        margin-bottom: 20px;
        span {
          margin-bottom: 20px;
          color: #02a7f0;
          font-size: 25px;
        }
      }
    }
    .img {
      width: 60px;
      position: absolute;
      bottom: 70px;
      right: 90px;
    }
  }
  .qiye {
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 600px;
    box-shadow: 0 2px 12px 0 rgb(0 0 0 / 10%);
    .list {
      display: flex;
      .listbox {
        margin-right: 15px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
      }
    }
  }
  .changsan {
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 600px;
    box-shadow: 0 2px 12px 0 rgb(0 0 0 / 10%);
    .text {
      p {
        font-size: 50px;
        font-weight: 900;
        color: #1d2b53;
        span {
          font-size: 30px;
          font-weight: normal;
        }
      }
      div {
        color: #f08300;
        font-size: 30px;
        font-weight: 600;
      }
    }
  }
  .swiper-ha {
    padding-top: 100px;
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 1000px;
    box-shadow: 0 2px 12px 0 rgb(0 0 0 / 10%);
    .swiper-container {
      width: 600px;
      height: 300px;
    }
    .logolist {
      width: 700px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
  }
  .foot {
    .text {
      width: 300px;
      text-align: center;
      margin: 0 auto;
      padding-top: 100px;
      h2 {
        font-size: 40px;
      }
      p {
        color: #027db4;
        font-size: 20px;
        margin: 20px 0;
      }
    }
  }
  .footer {
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 300px;
    .icon {
      display: flex;
      flex-direction: column;
      align-items: center;
      .icon1 {
        img {
          width: 30px;
        }
      }
      .icon2 {
        display: flex;
        justify-content: space-between;
        width: 100px;
        img {
          width: 30px;
        }
      }
    }
    .txt {
      display: flex;
      align-items: center;
      img {
        margin-left: 100px;
      }
    }
  }
}
</style>
