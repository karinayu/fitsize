<template>
    <el-main class="fitting-room">
        <iframe width="100%" height="95%" src="https://style.clo-set.com/fitting/u%2F2Cn2ZJ0O1qde2BlKWErg%3D%3D?ui_shopping_bag=0&ui_logo=0&size_idx=1" allow="allow-same-origin allow-scripts"></iframe>
      </el-main>
</template>
<script>
  var tag = document.createElement('script');
  tag.src = "https://files.clo-set.com/dist/fitting_viewer_iframe_api/0.0.2/closet_fitting_viewer_iframe_api.js";
  var firstScriptTag = document.getElementsByTagName('script')[0];
  firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);
  tag.onload = () => {
    function likeHandler(data){
      localStorage.setItem('data_key', JSON.stringify(data));
    }

    const handleDetail = (info) => {
      console.log(info);
      localStorage.setItem('info_key', JSON.stringify(info));
    }
    console.log(window.ClosetFittingIframeAPI);

    window.ClosetFittingIframeAPI.addEventListener('createAvatar', handleDetail);
    window.ClosetFittingIframeAPI.addEventListener('clickLike', likeHandler);
  }
export default {
  name: "Fitting-room",
}
</script>
