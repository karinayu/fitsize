<template>
  <el-main>
    <div class="main-banner block favourite"> 
      <div>
        <img :src="$auth.user.picture">
        <h4>{{ $auth.user.name }}</h4>
        <p>{{ $auth.user.email }}</p>
      </div>
      <el-divider></el-divider>
      <div class="favs">
        <div v-if="data.value!=false" class="fav-item">
          <p v-if="JSON.stringify(data.data.sizeIndex, 'Ничего не выбрано', '  ')==0">Выбранный размер: XXS</p>
          <p v-if="JSON.stringify(data.data.sizeIndex, 'Ничего не выбрано', '  ')==1">Выбранный размер: XS</p>
          <p v-if="JSON.stringify(data.data.sizeIndex, 'Ничего не выбрано', '  ')==2">Выбранный размер: S</p>
          <p v-if="JSON.stringify(data.data.sizeIndex, 'Ничего не выбрано', '  ')==3">Выбранный размер: M</p>
          <p v-if="JSON.stringify(data.data.colorwayIndex, 'Ничего не выбрано', '  ')==0">Выбранный цвет:
            <img src="../img/0.png" alt='pink'>
          </p>
          <p v-if="JSON.stringify(data.data.colorwayIndex, 'Ничего не выбрано', '  ')==1">Выбранный цвет:
            <img src="../img/1.png" style="height: 100px; width:100px">
          </p>
          <p v-if="JSON.stringify(data.data.colorwayIndex, 'Ничего не выбрано', '  ')==2">Выбранный цвет:
            <img src="../img/2.png" style="height: 100px; width:100px">
          </p>
        </div>
      </div>
    </div>
  </el-main>
</template>
<script>

export default {
  name: "Favourite",
  data() {
    const data = localStorage.getItem('data_key');
    return {
      data: JSON.parse(data),
    }
  }
}
</script>
