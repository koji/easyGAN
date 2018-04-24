<template>
    <div>
        <p>These gif are made by iamges which are related to art.</p>
        <a href="https://github.com/sleepy-maker/Art-DCGAN">Art-GAN</a>
        <br>
        <br>
            <img v-for="gif in gifs" :src="gif.url" />
    </div>
</template>

<script>
export default {
  data() {
    return {
      gifs: [
        {
          url: require("../../assets/art.gif")
        },
        {
          url: require("../../assets/generative_ver.gif")
        }
      ]
    };
  }
};
</script>
