<template>
  <el-dialog
  :visible.sync="dialogVisible"
  width="50%"
  :before-close="handleClose">
    <el-form :model="form">
      <h2>Выберите длительность, дату и время</h2>
      <el-form-item>
        <el-radio-group v-model="form.duration">
          <el-radio label="30 мин"></el-radio>
          <el-radio label="1 час"></el-radio>
          <el-radio label="2 часа"></el-radio>
        </el-radio-group>
      </el-form-item>
      <el-date-picker
      v-model="value1"
      type="date"
      placeholder="Выберите дату">
    </el-date-picker>
    <el-time-select
    v-model="value"
    :picker-options="{
      start: '12:00',
      step: '00:30',
      end: '19:30'
    }"
    placeholder="Выберите время">
</el-time-select>
    </el-form>
    <span slot="footer" class="dialog-footer">
      <div class="payment">
        <p>К оплате</p>
        <span>2200 р.</span>
      </div>
      <el-button class="black" @click="dialogVisible = false">Оплатить и забронировать</el-button>
    </span>
</el-dialog>
</template>
<script>
  export default {
    name: 'Login',
    data() {
      return {
        dialogVisible: false,
        value: '',
        pickerOptions: {
          disabledDate(time) {
            return time.getTime() > Date.now();
          },
          },
        value1: '',
      };
    }
  }
</script>