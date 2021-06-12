<template>
    <div class="course-list">
      <CoursePreview
      />
    </div>
</template>
<script>
import CoursePreview from "./CoursePreview";
export default {
    name: "CourseList",
    components: {
    CoursePreview
  },
}
</script>