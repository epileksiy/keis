<template>
    <section>
      <div>
        <span></span>
        <span></span>
      </div>
      <div>
        <span></span>
        <span></span>
      </div>
      <div>
        <span></span>
        <span></span>
      </div>
      <div>
        <span></span>
        <span></span>
      </div>
    </section>
</template>

<script>
    export default {
        name: "hypno"
    }
</script>

<style scoped>
  BODY {
    background: black;
    overflow: hidden;
    font-size: 16px;
  }

  SECTION {
    position: relative;
    width: 15em;
    height: 15em;
    margin: 5em auto;
    animation: hypnosis 5s infinite linear;
    border: 1px dotted #444;
    border-radius: 50%;
    display: flex;
  }

  DIV {
    position: relative;
    width: 10em;
    height: 10em;
    transform-origin: 5em 5em;
    border-radius: 50%;
    font-size: 1.5em;
  }
  DIV:nth-child(2),
  DIV:nth-child(3),
  DIV:nth-child(4) {
    position: absolute;
    top: 0;
    left: 0;
  }
  DIV:nth-child(3),
  DIV:nth-child(4) {
    animation: hypnosis 3s linear infinite reverse;
  }
  DIV:nth-child(2) {
    transform: rotate(90deg);
  }
  DIV:nth-child(3) {
    animation-delay: -1.5s;
  }
  DIV:nth-child(4) {
    animation-delay: -3s;
  }

  SPAN,
  SPAN:before,
  SPAN:after {
    position: absolute;
    display: block;
    border-top: .3em solid white;
    border-radius: 50%;
    animation: color 10s infinite;
  }
  SPAN {
    top: 0em;
    width: 9em;
    height: 9em;
    transform-origin: 5em 2.9em;
  }
  SPAN:before,
  SPAN:after {
    content: "";
  }
  SPAN:before {
    right: .1em;
    top: -.2em;
    width: 8em;
    height: 8em;
    border: 0 solid white;
    border-width:  0 .3em 0 0;
  }
  SPAN:after {
    right: .4em;
    bottom: 1.2em;
    width: 6.5em;
    height: 6.5em;
    border: 0 solid white;
    border-width: 0 0 .3em 0;
  }
  SPAN:nth-child(2) {
    transform-origin: 8.3em 4.8em;
    transform: rotate(-90deg);
    font-size: .6em;
  }
  SPAN:nth-child(3) {
    transform-origin: 8em 8.7em;
    transform: rotate(180deg);
    font-size: .2em;
  }

  DIV:nth-child(2) SPAN,
  DIV:nth-child(2) SPAN:before,
  DIV:nth-child(2) SPAN:after {
    border-color: skyblue;
    animation-delay: 7.5s;
  }
  DIV:nth-child(3) SPAN,
  DIV:nth-child(3) SPAN:before,
  DIV:nth-child(3) SPAN:after {
    border-color: crimson;
    animation-delay: 5s;
  }
  DIV:nth-child(4) SPAN,
  DIV:nth-child(4) SPAN:before,
  DIV:nth-child(4) SPAN:after {
    border-color: gold;
    animation-delay: 2.5s;
  }

  @keyframes hypnosis {
    100% {
      transform: rotate(360deg);
    }
  }

  @keyframes color {
    10% {
      border-color: purple;
    }
    20% {
      border-color: gold;
    }
    30% {
      border-color: crimson;
    }
    40% {
      border-color: chartreuse;
    }
    50% {
      border-color: orangereg;
    }
    60% {
      border-color: steelblue;
    }
    70% {
      border-color: orchid;
    }
    80% {
      border-color: orange;
    }
    90% {
      border-color: aquamarine;
    }
  }
</style>
