import { default } from '../components/Header.vue';
<template>
  <div class="about">
    <el-container>
      <el-header>
        <Header :flag="false" />
      </el-header>
      <el-main>
        <el-card>
          <h2>技术云智慧园区管理系统</h2>
          <p style="margin:50px 20px">技术云智慧园区管理系统提供免费试用申请， 请通过填写如下内容， 进行申请试用</p>
          <el-form
            :rules="rules"
            label-position="top"
            label-width="50px"
            :model="formLabelAlign"
          >
            <el-form-item
              label="您的名称"
              prop="name"
            >
              <el-input
                v-model="formLabelAlign.name"
                placeholder="希望我们如何称呼您"
              ></el-input>
            </el-form-item>
            <el-form-item
              label="手机"
              prop="region"
            >
              <el-input
                v-model="formLabelAlign.region"
                placeholder="顾问将于 1-2 个工作日内给您致电"
              ></el-input>
            </el-form-item>
            <el-form-item
              label="园区名称"
              prop="type"
            >
              <el-input
                v-model="formLabelAlign.type"
                placeholder="请提供完整的工商注册名称， 否则可能导致预约失败"
              ></el-input>
            </el-form-item>
            <el-form-item
              label="所属城市"
              prop="city"
            >
              <el-select
                v-model="formLabelAlign.city"
                placeholder="请选择省份-城市"
              >
                <el-option
                  v-for="item in options"
                  :key="item.value"
                  :label="item.label"
                  :value="item.value"
                >
                </el-option>
              </el-select>
            </el-form-item>
            <el-form-item label="想了解的内容 (可多选)">
              <el-checkbox-group v-model="checkList">
                <el-checkbox label="项目管理"></el-checkbox>
                <el-checkbox label="业务流程"></el-checkbox>
                <el-checkbox label="研发管理"></el-checkbox>
                <el-checkbox label="目标管理"></el-checkbox>
                <el-checkbox label="任务追踪"></el-checkbox>
                <el-checkbox label="敏捷开发"></el-checkbox>
                <el-checkbox label="需求管理"></el-checkbox>
                <el-checkbox label="跨部门协同"></el-checkbox>
                <el-checkbox label="知识库"></el-checkbox>
                <el-checkbox label="其他"></el-checkbox>
              </el-checkbox-group>
            </el-form-item>
            <el-form-item>
              <el-button
                type="primary"
                @click="onSubmit"
              >提交</el-button>
            </el-form-item>
          </el-form>
        </el-card>
      </el-main>
    </el-container>
  </div>
</template>
<script>
import Header from "../components/Header.vue";
export default {
  data() {
    return {
      formLabelAlign: {
        name: "",
        region: "",
        type: "",
        city: "",
      },
      options: [
        {
          label: "北京",
          value: 1,
        },
        {
          label: "深圳",
          value: 2,
        },
      ],
      checkList: ["其他"],
      rules: {
        name: [{ required: true, message: "请输入活动名称", trigger: "blur" }],
        region: [
          { required: true, message: "请选择活动区域", trigger: "blur" },
        ],
        city: [{ required: true, message: "请选择活动区域", trigger: "blur" }],
        type: [
          {
            type: "array",
            required: true,
            message: "请至少选择一个活动性质",
            trigger: "change",
          },
        ],
      },
    };
  },
  components: {
    Header,
  },
};
</script>
<style lang="scss" scoped>
.about {
  .el-main {
    background: #f2f3f5;
    height: 100vh;
  }
}
</style>
