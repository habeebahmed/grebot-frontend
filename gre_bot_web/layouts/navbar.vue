<template>
   <el-container>
        <el-aside width="200px">
            <el-col >
            <el-menu
                default-active="1"
                class="el-menu-vertical-demo"
                @open="handleOpen"
                @close="handleClose"
                background-color="#545c64"
                text-color="#fff"
                active-text-color="#ffd04b">
                <!-- <el-submenu index="1">
                    <template slot="title">
                    <i class="el-icon-location"></i>
                    <span>Navigator One</span>
                    </template>
                    <el-menu-item-group title="Group One">
                    <el-menu-item index="1-1">item one</el-menu-item>
                    <el-menu-item index="1-2">item one</el-menu-item>
                    </el-menu-item-group>
                    <el-menu-item-group title="Group Two">
                    <el-menu-item index="1-3">item three</el-menu-item>
                    </el-menu-item-group>
                    <el-submenu index="1-4">
                    <template slot="title">item four</template>
                    <el-menu-item index="1-4-1">item one</el-menu-item>
                    </el-submenu>
                </el-submenu> -->
                <el-menu-item index="1">
                    <i class="el-icon-info"></i>
                    <span>User Info</span>
                </el-menu-item>
                <el-menu-item index="2">
                    <i class="el-icon-tickets"></i>
                    <span>Statistics</span>
                </el-menu-item>
                <!-- <el-menu-item index="3" disabled>
                    <i class="el-icon-document"></i>
                    <span>Navigator Three</span>
                </el-menu-item> -->
                <el-menu-item index="3">
                    <i class="el-icon-rank"></i>
                    <span>Broadcast</span>
                </el-menu-item>
                <el-menu-item index="4">
                    <i class="el-icon-warning"></i>
                    <span>Logout</span>
                </el-menu-item>
            </el-menu>
        </el-col>
        </el-aside>
        <el-container>
            <el-header>Header</el-header>
            <el-main> <nuxt/></el-main>
            <el-footer>Footer</el-footer>
        </el-container>
    </el-container>
</template>

<style scoped>
.el-menu-vertical-demo {
  height: 947px;
}
.el-header, .el-footer {
    background-color: #B3C0D1;
    color:#fff;
    text-align: center;
    line-height: 60px;
  }
  
  .el-aside {
    background-color: #545c64;
    color: #333;
    text-align: center;
    line-height: 200px;
  }
  
  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
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

</style>