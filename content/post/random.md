---
title: "Random"
date: 2018-08-18T11:27:13-02:00
draft: yes
---

<style type="text/css">
	body {
	  font-size: 14px;
	  font-weight: 500;
	  -webkit-font-smoothing: antialiased;
	}

	.title {
	  font-family: "Raleway";
	  font-size: 24px;
	  font-weight: 700;
	  color: #5D4037;
	  text-align: center;
	}

	p {
	  line-height: 1.5em;
	}

	h1 + p, p + p {
	  margin-top: 10px;
	}

	.container {
	  /*padding: 40px 80px;*/
	  display: flex;
	  flex-wrap: wrap;
	  justify-content: space-between;
	}

	.card-wrap {
	  margin: 10px;
	  -webkit-transform: perspective(800px);
	          transform: perspective(800px);
	  -webkit-transform-style: preserve-3d;
	          transform-style: preserve-3d;
	  cursor: pointer;
	}
	.card-wrap:hover .card-info {
	  -webkit-transform: translateY(0);
	          transform: translateY(0);
	}
	.card-wrap:hover .card-info p {
	  opacity: 1;
	}
	.card-wrap:hover .card-info, .card-wrap:hover .card-info p {
	  transition: 0.6s cubic-bezier(0.23, 1, 0.32, 1);
	}
	.card-wrap:hover .card-info:after {
	  transition: 5s cubic-bezier(0.23, 1, 0.32, 1);
	  opacity: 1;
	  -webkit-transform: translateY(0);
	          transform: translateY(0);
	}
	.card-wrap:hover .card-bg {
	  transition: 0.6s cubic-bezier(0.23, 1, 0.32, 1), opacity 5s cubic-bezier(0.23, 1, 0.32, 1);
	  opacity: 0.8;
	}
	.card-wrap:hover .card {
	  transition: 0.6s cubic-bezier(0.23, 1, 0.32, 1), box-shadow 2s cubic-bezier(0.23, 1, 0.32, 1);
	  box-shadow: rgba(255, 255, 255, 0.2) 0 0 40px 5px, white 0 0 0 1px, rgba(0, 0, 0, 0.66) 0 30px 60px 0, inset #333 0 0 0 5px, inset white 0 0 0 6px;
	}

	.card {
	  position: relative;
	  flex: 0 0 240px;
	  width: 240px;
	  height: 320px;
	  background-color: #333;
	  overflow: hidden;
	  border-radius: 10px;
	  box-shadow: rgba(0, 0, 0, 0.66) 0 30px 60px 0, inset #333 0 0 0 5px, inset rgba(255, 255, 255, 0.5) 0 0 0 6px;
	  transition: 1s cubic-bezier(0.445, 0.05, 0.55, 0.95);
	}

	.card-bg {
	  opacity: 0.5;
	  position: absolute;
	  /*top: -20px;
	  left: -20px;*/
	  width: 100%;
	  height: 100%;
	  /*padding: 20px;*/
	  background-repeat: no-repeat;
	  background-position: center;
	  background-size: cover;
	  transition: 1s cubic-bezier(0.445, 0.05, 0.55, 0.95), opacity 5s 1s cubic-bezier(0.445, 0.05, 0.55, 0.95);
	  pointer-events: none;
	}

	.card-info {
	  padding: 20px;
	  position: absolute;
	  bottom: 0;
	  color: #fff;
	  -webkit-transform: translateY(40%);
	          transform: translateY(40%);
	  transition: 0.6s 1.6s cubic-bezier(0.215, 0.61, 0.355, 1);
	}
	.card-info p {
	  opacity: 0;
	  color: white;
	  text-shadow: black 0 2px 3px;
	  transition: 0.6s 1.6s cubic-bezier(0.215, 0.61, 0.355, 1);
	}
	.card-info * {
	  position: relative;
	  z-index: 1;
	}
	.card-info:after {
	  content: '';
	  position: absolute;
	  top: 0;
	  left: 0;
	  z-index: 0;
	  width: 100%;
	  height: 100%;
	  background-image: linear-gradient(to bottom, transparent 0%, rgba(0, 0, 0, 0.6) 100%);
	  background-blend-mode: overlay;
	  opacity: 0;
	  -webkit-transform: translateY(100%);
	          transform: translateY(100%);
	  transition: 5s 1s cubic-bezier(0.445, 0.05, 0.55, 0.95);
	}

	.card-info h1 {
	  font-size: 28px;
	  font-weight: 700;
	  text-shadow: rgba(0, 0, 0, 0.5) 0 10px 10px;
	}
</style>

<div class="">
	<center>
		<h3>Random</h3>
	</center>
	<br>
	<br>
	<div id="app" class="container">
	  <card data-image="https://media.giphy.com/media/PQMTllhpoIBfRTjEyk/giphy.gif">
	    <h1 slot="header">IKEA Fun</h1>
	    <p slot="content">Hacking IKEA stuff for measuring Air Quality (ESP8266 + Proximity Sensors + Led Ring + 3D Printing) </p>
	  </card>
	  <card data-image="https://media.giphy.com/media/X7qVPGwHqKktUlrK3q/giphy.gif">
	    <h1 slot="header">Tree of Ideas</h1>
	    <p slot="content">Record + Manage Playlist + Transducers, everything over Raspberry Pi</p>
	  </card>
	  <card data-image="https://media.giphy.com/media/1i4tj1iTwSAco9KUzL/giphy.gif">
	    <h1 slot="header">Lazy</h1>
	    <p slot="content">Lazyness and creativity. Totally related.</p>
	  </card>
	  <card data-image="https://media.giphy.com/media/67ThDYMzoGWFk7NKk7/giphy.gif">
	    <h1 slot="header">Led Bag</h1>
	    <p slot="content">Sewing + Fiber Optics + LEDs. Idea by me and Aline. All the maker stuff: alinemartinez.io</p>
	  </card>
	</div>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/vue/2.0.1/vue.min.js"></script>
<script type="text/javascript">
	Vue.config.devtools = true;

	Vue.component('card', {
	  template: '\n    <div class="card-wrap"\n      @mousemove="handleMouseMove"\n      @mouseenter="handleMouseEnter"\n      @mouseleave="handleMouseLeave"\n      ref="card">\n      <div class="card"\n        :style="cardStyle">\n        <div class="card-bg" :style="[cardBgTransform, cardBgImage]"></div>\n        <div class="card-info">\n          <slot name="header"></slot>\n          <slot name="content"></slot>\n        </div>\n      </div>\n    </div>',
	  mounted: function mounted() {
	    this.width = this.$refs.card.offsetWidth;
	    this.height = this.$refs.card.offsetHeight;
	  },
	  props: ['dataImage'],
	  data: function data() {return {
	      width: 0,
	      height: 0,
	      mouseX: 0,
	      mouseY: 0,
	      mouseLeaveDelay: null };},

	  computed: {
	    mousePX: function mousePX() {
	      return this.mouseX / this.width;
	    },
	    mousePY: function mousePY() {
	      return this.mouseY / this.height;
	    },
	    cardStyle: function cardStyle() {
	      var rX = this.mousePX * 30;
	      var rY = this.mousePY * -30;
	      return {
	        transform: 'rotateY(' + rX + 'deg) rotateX(' + rY + 'deg)' };

	    },
	    cardBgTransform: function cardBgTransform() {
	      var tX = this.mousePX * -1;
	      var tY = this.mousePY * -1;
	      return {
	        transform: 'translateX(' + tX + 'px) translateY(' + tY + 'px)' };

	    },
	    cardBgImage: function cardBgImage() {
	      return {
	        backgroundImage: 'url(' + this.dataImage + ')' };

	    } },

	  methods: {
	    handleMouseMove: function handleMouseMove(e) {
	      this.mouseX = e.pageX - this.$refs.card.offsetLeft - this.width / 2;
	      this.mouseY = e.pageY - this.$refs.card.offsetTop - this.height / 2;
	    },
	    handleMouseEnter: function handleMouseEnter() {
	      clearTimeout(this.mouseLeaveDelay);
	    },
	    handleMouseLeave: function handleMouseLeave() {var _this = this;
	      this.mouseLeaveDelay = setTimeout(function () {
	        _this.mouseX = 0;
	        _this.mouseY = 0;
	      }, 1000);
	    } } });

	var app = new Vue({
  		el: '#app' });
</script>

