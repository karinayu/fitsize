<template>
  <el-container id="app" :direction="horizontal">
    <el-header>
          <el-menu :default-active="activeIndex" class="el-menu-demo" router="true" mode="horizontal">
            <el-menu-item class="home" index="/">FitSize</el-menu-item>
            <el-menu-item index="/fitting-room">Примерочная</el-menu-item>
            <el-menu-item v-if="$auth.isAuthenticated" index="/favourite">Избранное</el-menu-item>
            <el-menu-item index="/faq">FAQ</el-menu-item>
            <el-menu-item index="/about">О нас</el-menu-item>
          <el-menu-item>
              <div v-if="!$auth.loading">
                  <!-- show login when not authenticated -->
                  <button class="gray" v-if="!$auth.isAuthenticated" @click="login">Войти</button>
                  <!-- show logout when authenticated -->
                  <button class="gray" v-if="$auth.isAuthenticated" @click="logout">Выйти</button>
              </div>
          </el-menu-item>
          </el-menu>
      </el-header>
    <router-view/>
    <el-footer height="30vh">
      <el-row type="flex" justify="space-between" border="solid">
        <el-col :span="8">
          <el-col :span="12">
            <el-row><router-link to="/fitting-room">Примерочная</router-link></el-row>
            <el-row><router-link v-if="$auth.isAuthenticated" to="/favourite">Избранное</router-link></el-row>
            <el-row><router-link to="/about">О нас</router-link></el-row>
          </el-col>
        </el-col>
      </el-row>
    </el-footer>
  </el-container>
</template>
<script>

export default {
  name: "App",
  components: {},
  methods: {
    // Log the user in
    login() {
      this.$auth.loginWithRedirect();
    },
    // Log the user out
    logout() {

      this.$auth.logout({
        returnTo: window.location.origin
      });
    }
  }
};
</script>