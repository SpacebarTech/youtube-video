// Put what you want to export in this file
<template lang="pug">

	.youtube-video(:style='{ maxHeight : `${height}px` }')
		iframe(
			v-if='videoId'
			:width='width'
			:height='height'
			v-bind:src="`https://www.youtube.com/embed/${videoId}`"
			frameborder="0"
			allowfullscreen
			ref='frame'
		)

</template>

<script>

  export default {

    props : {
      videoId : {
        type : String
      },
      height : {
        default : 300
      },
      width : {
        default : 500
      }
    },
  }

</script>


<style lang="scss">

  $lightGrey : #ebf1f7;

  .youtube-video {
    background-color: $lightGrey;
  }

</style>

