<template>
  <div>
    <CallToAction></CallToAction>
    <Navbar></Navbar>
    <div class="assessment">
      <div class="assessment__con">
        <h1 class="assessment__con--title text-center">
          <!-- How will COVID-19 affect your business? -->
          Assessment
        </h1>
        <div
          class="assessment__con--info text-center"
        >Find out how COVID-19 may affect your cashflow</div>
      </div>
    </div>
    <Analytics></Analytics>
    <div class="cta-assessment">
      This cashflow forecasting tool was created by the team at Fostrum
      Financial Technologies. Learn more about other cool projects we're up to
      <a
        href="http://www.fostrum.com"
      >
        <b>here</b>
      </a>.
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
const CallToAction = () => import("@/components/CallToAction.vue");
const Navbar = () => import("@/components/Navbar.vue");
const Analytics = () => import("@/components/Analytics.vue");
const Footer = () => import("@/components/Footer.vue");

export default {
  name: "Assessment",
  components: {
    CallToAction,
    Navbar,
    Analytics,
    Footer
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.assessment {
  width: 100%;
}
.assessment__con {
  margin: 1em 1em;
}
.assessment__con--title {
  font-size: 3em;
  margin-top: 0em;
}

.assessment__con--values {
  font-weight: bold;
}
.cta-assessment {
  margin-top: 4em;
  padding: 0em 1em;
}

@media screen and (min-width: 768px) {
  .cta-assessment {
    margin-top: 4em;
    width: 768px;
    margin: 0 auto;
    padding: 0em 0em;
  }
}
</style>
