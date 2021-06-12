<template>
    <el-row>
        <router-link to="/advices/advice-page">
            <el-col :span="6" class="advice-preview card">
                <div class="tags">
                    <p># Беременность </p>
                    <p>Бесплатно</p>
                </div>
                <div class="info">
                    <div class="duration">1 ч 20 мин  •  152 просмотра</div>
                    <div class="video-title">Название видео</div>
                </div>
            </el-col>
        </router-link>
        <router-link to="/advices/advice-page">
            <el-col :span="6" class="advice-preview card">
                <div class="tags">
                    <p># Беременность </p>
                    <p>Бесплатно</p>
                </div>
                <div class="info">
                    <div class="duration">1 ч 20 мин  •  152 просмотра</div>
                    <div class="video-title">Название видео</div>
                </div>
            </el-col>
        </router-link>
        <router-link to="/advices/advice-page">
            <el-col :span="6" class="advice-preview card">
                <div class="tags">
                    <p># Беременность </p>
                    <p>Бесплатно</p>
                </div>
                <div class="info">
                    <div class="duration">1 ч 20 мин  •  152 просмотра</div>
                    <div class="video-title">Название видео</div>
                </div>
            </el-col>
        </router-link>
    </el-row>
</template>
<script>
export default {
    name: "AdvicePreview"
}
</script>