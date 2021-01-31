<template>
  <div id="app" class="bg-gray-900 h-screen">
    <headline></headline>
    <navigation></navigation>

    <div class="px-12 bg-gray-800 mx-24">
      <div class="mx-auto pt-6 ">
        <transition
        mode="out-in"
        enter-active-class="animate__animated animate__fadeInLeft! "
        leave-active-class="animate__animated animate__fadeOut">
          <router-view/>

        </transition>
      </div>
    </div>



  </div>
</template>

<style>

</style>
<script>
import Headline from "@/components/Headline";
import Navigation from "@/components/navigation";
export default {
  components: {Navigation, Headline}
}
</script>