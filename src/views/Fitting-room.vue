<template>
    <el-main class="fitting-room">
        <iframe width="100%" height="95%" src="https://style.clo-set.com/fitting/u%2F2Cn2ZJ0O1qde2BlKWErg%3D%3D?ui_shopping_bag=0&ui_logo=0" allow="allow-same-origin allow-scripts"></iframe>
      </el-main>
</template>
<script>
  import {FAVORITE_KEY} from './../settings.js';

  var tag = document.createElement('script');
  tag.src = "https://files.clo-set.com/dist/fitting_viewer_iframe_api/0.0.2/closet_fitting_viewer_iframe_api.js";
  var firstScriptTag = document.getElementsByTagName('script')[0];
  firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);
  tag.onload = () => {
    function likeHandler(data){
      localStorage.setItem(FAVORITE_KEY, JSON.stringify(data));
    }

    const handleKek = (...data) => {
      console.log(data);
    }
    console.log(window.ClosetFittingIframeAPI);

    // eslint-disable-next-line no-undef
    window.ClosetFittingIframeAPI.addEventListener('kek', handleKek);

    // eslint-disable-next-line no-undef
    window.ClosetFittingIframeAPI.addEventListener('clickLike', likeHandler);
  }
export default {
  name: "Fitting-room",
}
</script>
