<template>
    <div class="profile">
        <h4>Данные профиля</h4>
        <el-card class="box-card">
            <div slot="header" class="clearfix">
                <img :src="$auth.user.picture">
                <div>{{ $auth.user.name }}</div>
                <div>{{ $auth.user.email }}</div>
                <el-button style="float: right; padding: 3px 0" type="text">Operation button</el-button>
            </div>
            <p>Рост: {{JSON.stringify(data.profile.height, 'не указано', '  ')}} см</p>
        <p>Вес: {{JSON.stringify(data.profile.weight, 'не указано', '  ')}} кг</p>
        <p>Дополнительная информация:{{JSON.stringify(data.profile, 'не указано', '  ')}}</p>
        </el-card>
    </div>
</template>
<script>
const defaultInfo = {
    profile: '',
}
export default {
    name: "Profile",
    data() {
    const info = localStorage.getItem('info_key');
    const detail = info ? JSON.parse(info) : defaultInfo;
    return detail;
    },
}
</script>
