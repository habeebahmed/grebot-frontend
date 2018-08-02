<template>
  <!-- <div class="container">
    <div class="box header">  
      <p class="hText">TOP SCORES</p>  
    </div>  
    <div class="box main"> 
      <div class="block">
        <el-container style="height: 770px;width: 640px; border: 1px solid #eee">
          <el-header style="text-align: center; font-size: 12px;background-color:grey;height:60px;">
            <span style="font-size:30px;color:rgb(235, 231, 16);">Data</span>
          </el-header>  
          <el-main>
            <el-table :data="tableData">
              <el-table-column prop="date" label="Date" width="100">
  
              </el-table-column>
  
              <el-table-column prop="name" label="Name" width="100">
  
              </el-table-column>
  
              <el-table-column prop="address" label="Address">
  
              </el-table-column>
  
            </el-table>
  
          </el-main>
  
        </el-container>
  
      </div>

      <div class="block">2</div>
  
      <div class="block">3</div>
  
    </div>
  
    <div class="box footer"></div>
  
  
  
  </div> -->
  <el-container>
    <el-header>Header</el-header>
    <el-main>
      <el-row>
        <el-col :span="8"><div class="grid-content bg-purple">hello</div></el-col>
        <el-col :span="8"><div class="grid-content bg-purple-light"></div></el-col>
        <el-col :span="8"><div class="grid-content bg-purple"></div></el-col>
      </el-row>
    </el-main>
    <el-footer>Footer</el-footer>
  </el-container>
</template>
<script>
export default {
  name: "score",
  data() {
    const item = {
      date: "2016-05-02",
      name: "Tom",
      address: "No. 189, Grove St, Los Angeles"
    };
    return {
      scores: [],
      tableData: Array(20).fill(item)
    };
  },

  methods: {}
};
</script>

<style scoped>
.container {
  display: flex;

  flex-direction: column;

  text-align: center;

  margin: 0 auto;

  justify-content: center;

  align-content: center;

  min-height: 945px;
}

.hText {
  padding: 20px;

  font-size: 20px;

  font-family: Arial, Helvetica, sans-serif;

  font-weight: bold;
}

.box {
  height: 50px;

  /* flex-basis: 300px; */
}

.header {
  background-color: blue;

  flex-grow: 1;
}

.main {
  background-color: red;

  flex-grow: 20;

  display: flex;
}

.block {
  border: 1px solid;

  flex-grow: 1;

  background-color: white;
}

.footer {
  background-color: greenyellow;

  flex-grow: 1;
}
.block {
  width: 300px;
}
.el-header,
.el-footer {
  background-color: #b3c0d1;
  color: #333;
  text-align: center;
  line-height: 60px;
}

.el-aside {
  background-color: #d3dce6;
  color: #333;
  text-align: center;
  line-height: 200px;
}

.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  line-height: 160px;
  min-height: 87.3vh;
}

body > .el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
.el-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
</style>
