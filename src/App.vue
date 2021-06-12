<template>
  <el-container id="app" :direction="horizontal">
    <el-header>
          <el-menu :default-active="activeIndex" class="el-menu-demo" router="true" mode="horizontal">
            <el-menu-item class="home" index="/">FitSize</el-menu-item>
            <el-menu-item index="/fitting-room">Примерочная</el-menu-item>
            <el-menu-item index="/favourite">Избранное</el-menu-item>
            <el-menu-item index="/about">О нас</el-menu-item>
            <!-- <el-menu-item class="login" index="/">Войти</el-menu-item> -->
          </el-menu>
      </el-header>
    <router-view/>
    <el-footer height="30vh">
      <el-row type="flex" justify="space-between" border="solid">
        <el-col :span="8">
          <el-col :span="12">
            <el-row class="tag">FitSize</el-row>
            <el-row><router-link to="/fitting-room">Примерочная</router-link></el-row>
            <el-row><router-link to="/favourite">Избранное</router-link></el-row>
            <el-row><router-link to="/about">О нас</router-link></el-row>
          </el-col>
        </el-col>
        <el-col :span="8">
          <el-row>
            <el-col :span="24">
              <button class="gray">Войти</button>
            </el-col>
          </el-row>
        </el-col>
      </el-row>

    </el-footer>
  </el-container>
</template>