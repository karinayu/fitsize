<template>
    <el-main class="article block">
        <router-link to="/blog">
        <el-page-header title="Вернуться">
        </el-page-header>
        </router-link>
        <div class="title">
            <h1>История моей второй беременности</h1>
            <p>Вы верите в чудеса? Сегодня хочу написать, каким чудесным образом нашему старшему сыну удалось появиться в нашей Жизни и «пробить» путь всем остальным. Да-да, не первому ребенку, а второму!</p>
        </div>
        <div class="content">
            <div class="text">
                <p>Мне сложно сказать, что в моих первых родах было не так, но я после них очень долго восстанавливалась. Почти месяц мне было тяжело ходить и разгибаться. Когда я закончила кормить грудью Лизу, у меня начались жуткие проблемы по гинекологии. </p>
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
    </el-main>
</template>
<script>
export default {
    name: "Article"
}
</script>