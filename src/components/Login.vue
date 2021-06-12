<template>
  <el-dialog
  :visible.sync="dialogVisible"
  width="50%"
  :before-close="handleClose">
    <h2>Введите код подтверждения</h2>
    <p>Введите ваш номер телефона</p>
    <form>
      <input type="phone" placeholder="+79">
      <button disabled class="gray">Войти</button>
    </form>
    <span slot="footer" class="dialog-footer">
      <el-button @click="dialogVisible = false">Закрыть</el-button>
    </span>
</el-dialog>
</template>
<script>
  export default {
    name: 'Login',
    data() {
      return {
        dialogVisible: false
      };
    }
  };
</script>