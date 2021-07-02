<template>
    <div class="profile">
        <h4>Данные профиля</h4>
        <img :src="$auth.user.picture">
        <h5>{{ $auth.user.name }}</h5>
        <p>{{ $auth.user.email }}</p>
        <p>Рост: {{JSON.stringify(data.profile.height, 'не указано', '  ')}} см</p>
        <p>Вес: {{JSON.stringify(data.profile.weight, 'не указано', '  ')}} кг</p>
        <p>Доп инфо: {{JSON.stringify(data.profile, 'не указано', '  ')}}</p>
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
