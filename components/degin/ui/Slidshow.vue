<template lang="pug">
  .slideshow
    .slideContents
      section#slide1
        img(src="img/top2.png")
      section#slide2
        img(src="img/top3.png")
      section#slide3
        img(src="img/top2.png")
      section#slide4
        img(src="img/top3.png")
      section#slide5
        img(src="img/top2.png")
</template>


<style lang="stylus">
.slideshow {
  position: relative;
  overflow: hidden;
}

.slideContents {
  position: relative;
  text-align: center;
  -webkit-user-select: none;
  user-select: none;

  img {
    width: 100%;
    height: 752px;
  }

  section {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
  }
}

.slideContents section img {
  max-width: 100%;
  box-sizing: border-box;
  vertical-align: middle;
}

.slideContents section {
  animation: autoplay 30s cubic-bezier(0.215, 0.61, 0.355, 1) infinite;
}

@keyframes autoplay {
  0%, 16%, 100% {
    transform: none;
  }

  20% {
    transform: translateX(-100%);
  }

  20.001%, 96% {
    transform: translateX(100%);
  }
}

.slideContents {
  #slide1 {
    position: relative;
    animation-delay: 0s;
  }

  #slide2 {
    animation-delay: -24s;
  }

  #slide3 {
    animation-delay: -18s;
  }

  #slide4 {
    animation-delay: -12s;
  }

  #slide5 {
    animation-delay: -6s;
  }
}
</style>