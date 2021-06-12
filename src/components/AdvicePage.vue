<template>
    <el-main class="advice-page">
        <router-link to="/advices">
        <el-page-header class="block" title="Назад">
        </el-page-header>
        </router-link>
        <div class="title block">
            <h1>Как подготовиться к родам?</h1>
            <p>Краткое описание видео. Важно следить, чтобы он соответствовал контенту. Краткое описание видео. Важно следить, чтобы он соответствовал контенту.</p>
        </div>
        <div class="info block">
            <div class="hashtags">
                <el-row :gutter="20">
                    <el-col :span="4"># 1-3 года</el-col>
                    <el-col :span="4"># 3-5 лет</el-col>
                    <el-col :span="4"># Подготовка</el-col>
                </el-row>
            </div>
            <div class="date-price">
                <div class="price">Бесплатно</div>
                <div class="date">
                    <p>2 месяца назад</p>
                    <p>•  152 просмотра</p>
                </div>
            </div>
        </div>
        <div class="video block">
            <video src=""></video>
        </div>
        <div class="about block">
            <div class="description">
                    <div class="name">Описание</div>
                    <div class="content">
                        <p>Текст описания. Важно следить, чтобы он соответствовал контенту. Текст описания. Важно следить, чтобы он соответствовал контенту. Текст описания. Важно следить, чтобы он соответствовал контенту. Текст описания. Важно следить, чтобы он соответствовал контенту..</p>
                        <button>Показать полностью</button>
                    </div>
            </div>
            <div class="description">
                    <div class="name">Задание</div>
                    <div class="content">
                        <p>Текст задания. Важно следить, чтобы он соответствовал контенту. Текст задания. Важно следить, чтобы он соответствовал контенту. Текст задания. Важно следить, чтобы он соответствовал контенту. Текст задания. Важно следить, чтобы он соответствовал контенту..</p>
                        <button>Показать полностью</button>
                    </div>
            </div>
        </div>
        <div class="infobox block">
            <div class="comments">
                <div class="title">
                    <h3>Комментарии</h3>
                    <p>3</p>
                </div>
                <input placeholder="Написать комментарий">
                <div class="filters">
                    <button>Популярные</button>
                    <button>Новые</button>
                </div>
                <el-divider></el-divider>
                <div class=""></div>
            </div>
            <div class="more">
                <p class="label">С этим видео смотрят</p>
                <div class="advices">
                    <AdvicePreview/>
                </div>
            </div>
        </div>
    </el-main>
</template>
<script>
import AdvicePreview from "./AdvicePreview";
export default {
    name: "AdvicePage",
    components: {
    AdvicePreview
    },
}
</script>