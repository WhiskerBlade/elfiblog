<template>
  <div class="p-4 sm:w-1/3 w-full max-w-md ">
    <div class="bg-white rounded-xl shadow-md overflow-hidden">
      <div class="bg-gray-200 h-48 flex items-center justify-center">
        <img class="w-32 h-32 object-cover rounded-full" :src="`https://static-cdn.jtvnw.net/jtv_user_pictures/${streamer.twitchGuid}-profile_image-150x150.png`" :alt="`${streamer.username} profile picture`">
      </div>
      <div class="px-4 py-2 flex justify-between">
        <h2 class="text-gray-800 text-xl font-bold troikaFont">{{ streamer.displayName }}</h2>
        <a :href="`https://www.twitch.tv/${streamer.username}`" target="_blank" class="text-indigo-600 hover:text-indigo-700 text-xl font-bold troikaFont">Check Now</a>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  props: ["streamer"],
};
</script>

<style></style>
