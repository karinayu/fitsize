<template>
    <el-row>
        <router-link to="/courses/course-page">
        <el-col :span="6" class="course-preview card">
            <div class="tags">
                <p># Беременность </p>
                <p>Бесплатно</p>
            </div>
            <div class="info">
                <div class="duration">30 уроков  •  2 месяца</div>
                <div class="course-title">Название курса</div>
            </div>
        </el-col>
        </router-link>
        <el-col :span="6" class="course-preview card">
            <div class="tags">
                <p># Беременность </p>
                <p>Бесплатно</p>
            </div>
            <div class="info">
                <div class="duration">30 уроков  •  2 месяца</div>
                <div class="course-title">Название курса</div>
            </div>
        </el-col>
        <el-col :span="6" class="course-preview card">
            <div class="tags">
                <p># Беременность </p>
                <p>Бесплатно</p>
            </div>
            <div class="info">
                <div class="duration">30 уроков  •  2 месяца</div>
                <div class="course-title">Название курса</div>
            </div>
        </el-col>
        <el-col :span="6" class="course-preview card">
            <div class="tags">
                <p># Беременность </p>
                <p>Бесплатно</p>
            </div>
            <div class="info">
                <div class="duration">30 уроков  •  2 месяца</div>
                <div class="course-title">Название курса</div>
            </div>
        </el-col>
    </el-row>
</template>
<script>
export default {
    name: "CoursePreview"
}
</script>