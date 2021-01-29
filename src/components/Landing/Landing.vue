<template>
  <div
    class="flex flex-center"
    :style="{
      backgroundImage: 'url(' + require('../../assets/hero.png') + ')',
      height: '100vh !important;'
    }"
  >
    <div class="row">
      <div class="col-12">
        <div
          class="text-h6"
          style="margin-top:-5rem;color:white; font-size:60px !important;font-style:bold;font-weight: 700"
        >
          You have what it takes.<br />
        </div>
        <div
          class="h6"
          style="text-align:center; color:white;font-size: 20px;font-weight: 400;margin-top:16px; margin-bottom:16px;"
        >
          Stadia turns the things you already own into portals to the biggest
          games.
        </div>
        <div style="text-align:center;">
          <q-btn
            style="background-image: linear-gradient(90deg, rgb(248, 73, 27) 0%, rgb(241, 47, 63) 50%, rgb(220, 24, 96) 100%);inline:1 Best Match .vORvAb.hXyPqf
linear-gradient(90deg, rgb(248, 73, 27) 0%, rgb(241, 47, 63) 50%, rgb(220, 24, 96) 100%);color:white;
height:50px;
"
            >Try Stadia Pro free for 1 month</q-btn
          >
        </div>
        <div
          style="text-align:center; color:white;margin-top:8px;margin-bottom:8px;"
        >
          <span style="font-size:16px;">
            €9.99/mo after trial, cancel anytime.
            <a
              style="color:white;cursor:pointer;"
              target="_blank"
              class="faBeld"
              href="https://support.google.com/stadia/answer/9789527"
              >Terms Apply.</a
            ></span
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {}
};
</script>

<style lang="scss">
.flex {
  height: 100vh;
}
</style>
