<template>
    <el-main class="video-lesson block">
        <router-link to="/courses/course-page">
        <el-page-header title="Вернуться">
        </el-page-header>
        </router-link>
        <div class="title">
            <h1>Видеоурок 3. 
                Как правильно разговаривать с ребенком</h1>
        </div>
        <div class="video-block">
            <video src=""></video>
            <div class="how-to">
                <div class="step">
                    <div>1</div>
                    <p>Посмотрите видео</p>
                </div>
                <div class="step">
                    <div>2</div>
                    <p>Выполните задание, написав ответ в комментариях</p>
                </div>
                <div class="step">
                    <div>3</div>
                    <p>Поставьте галочку “Выполняю задание”</p>
                </div>
            </div>
            <div class="about">
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
            <div class="infobox">
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
            </div>
        </div>
    </el-main>
</template>
<script>
export default {
    name: "VideoLesson"
}
</script>