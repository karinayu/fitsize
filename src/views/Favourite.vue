<template>
  <el-main>
    <div class="main-banner block favourite"> 
      <div>
        <img :src="$auth.user.picture">
        <h2>{{ $auth.user.name }}</h2>
        <p>{{ $auth.user.email }}</p>
      </div>
      <div class="favs">
        <div class="fav-item">{{ $auth.user.name }}</div>
      </div>
    </div>
  </el-main>
</template>
<script>
export default {
  name: "Favourite",
}
</script>
