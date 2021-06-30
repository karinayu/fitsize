<template>
  <el-main>
    <div class="main-banner block">
            <div>
              <h1>FitSize</h1>
              <p>Наша миссия - обеспечить лучший опыт онлайн-покупок с помощью 3D-решений, помогая производителям увеличить продажи и сократить количество возвратов.</p>
              <p>С помощью FitSize производители одежды могут создавать потрясающий цифровой опыт покупок с помощью современной 3D-визуализации и возможности виртуальной примерки одежды.</p>
            </div>
            <img src="../img/model.png" alt="3d model">
    </div>
  </el-main>
</template>
<script>

export default {
  name: "Home",
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