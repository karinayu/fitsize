<template>
  <el-main>
    <div class="main-banner block favourite"> 
      <router-view></router-view>
      <el-divider></el-divider>
      <div class="favs">
        <div class="fav-item">
          <p v-if="JSON.stringify(data.sizeIndex, 'Ничего не выбрано', '  ')==0">Выбранный размер: XXS</p>
          <p v-if="JSON.stringify(data.sizeIndex, 'Ничего не выбрано', '  ')==1">Выбранный размер: XS</p>
          <p v-if="JSON.stringify(data.sizeIndex, 'Ничего не выбрано', '  ')==2">Выбранный размер: S</p>
          <p v-if="JSON.stringify(data.sizeIndex, 'Ничего не выбрано', '  ')==3">Выбранный размер: M</p>
          <p v-if="JSON.stringify(data.sizeIndex, 'Ничего не выбрано', '  ')==4">Выбранный размер: L</p>
          <p v-if="JSON.stringify(data.sizeIndex, 'Ничего не выбрано', '  ')==5">Выбранный размер: XL</p>
          <p v-if="JSON.stringify(data.colorwayIndex, 'Не выбрано', '  ')==0">Выбранный цвет:
            <img src="../img/0.png" alt='beige'/>
          </p>
          <p v-if="JSON.stringify(data.colorwayIndex, 'Не выбрано', '  ')==1">Выбранный цвет:
            <img src="../img/1.png" alt='black&white'/>
          </p>
          <p v-if="JSON.stringify(data.colorwayIndex, 'Не выбрано', '  ')==2">Выбранный цвет:
            <img src="../img/2.png" alt='pink'/>
          </p>
        </div>
      </div>

    </div>
  </el-main>
</template>
<script>
const defaultData = {
  sizeIndex: '',
  colorwayIndex: '',
  value: false,
}
export default {
  name: "Favourite",
  data() {
    const data = localStorage.getItem('data_key');
    const parsed = data ? JSON.parse(data) : defaultData;
    return parsed;
  },
}
</script>
