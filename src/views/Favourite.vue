<template>
  <el-main>
    <div class="main-banner block favourite"> 
      <div>
        <img :src="$auth.user.picture">
        <h2>{{ $auth.user.name }}</h2>
        <p>{{ $auth.user.email }}</p>
      </div>
      <div class="favs">
        <div v-if="data.value!=false" class="fav-item">
          <p v-if="JSON.stringify(data.data.sizeIndex, 'Ничего не выбрано', '  ')==0">Выбранный размер: XXS</p>
          <p v-if="JSON.stringify(data.data.sizeIndex, 'Ничего не выбрано', '  ')==1">Выбранный размер: XS</p>
          <p v-if="JSON.stringify(data.data.sizeIndex, 'Ничего не выбрано', '  ')==2">Выбранный размер: S</p>
          <p v-if="JSON.stringify(data.data.sizeIndex, 'Ничего не выбрано', '  ')==3">Выбранный размер: M</p>
          <p v-if="JSON.stringify(data.data.colorwayIndex, 'Ничего не выбрано', '  ')==0">Выбранный цвет:
            <img scr="../img/model.png">
          </p>
          <p v-if="JSON.stringify(data.data.colorwayIndex, 'Ничего не выбрано', '  ')==1">Выбранный цвет:
            <img scr="../img/1.png" style="height: 100px; width:100px">
          </p>
          <p v-if="JSON.stringify(data.data.colorwayIndex, 'Ничего не выбрано', '  ')==2">Выбранный цвет:
            <img scr="../img/2.png" style="height: 100px; width:100px">
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
