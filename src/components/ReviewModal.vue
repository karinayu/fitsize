<template>
  <el-dialog :visible.sync="dialogFormVisible">
    <h2>Оставить отзыв</h2>
    <p>Напишите, что думаете по поводу курсов, клубов или обучающих видео</p>
    <el-form :model="form">
      <el-form-item label="Как вас зовут" :label-width="formLabelWidth">
        <el-input v-model="form.name" placeholder="Фамилия Имя"></el-input>
      </el-form-item>
      <el-form-item label="Ссылка на Facebook, Instagram или VK" :label-width="formLabelWidth">
        <el-input v-model="form.media" placeholder="Чтобы другие пользователи видели, что вы реальный человек">
        </el-input>
      </el-form-item>
      <el-form-item label="Текст отзыва" :label-width="formLabelWidth">
        <el-input v-model="form.text" placeholder="Начните вводить.."></el-input>
      </el-form-item>
    </el-form>
    <span slot="footer" class="dialog-footer">
      <button class="black" @click="dialogFormVisible = false">Отправить</button>
    </span>
  </el-dialog>
</template>
<script>
export default {
    name: 'ReviewModal',
    data() {
      return {
        dialogFormVisible: false,
        form: {
          name: '',
          region: '',
          date1: '',
          date2: '',
          delivery: false,
          type: [],
          resource: '',
          desc: ''
        },
        formLabelWidth: '120px'
      };
    }
  };
</script>   
