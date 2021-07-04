<template>
  <div class="details-grid">
      <div class="details-box">
          <h5>IP ADDRESS</h5>
          <h2>192.212.174.101</h2>
      </div>
      <div class="details-box box-border-left">
          <h5>LOCATION</h5>
          <h2>Brooklyn, NY 10001</h2>
      </div>
      <div class="details-box box-border-left">
          <h5>TIMEZONE</h5>
          <h2>UTC -05:00</h2>
      </div>
      <div class="details-box box-border-left">
          <h5>ISP</h5>
          <h2>SpaceX Starlink</h2>
      </div>
  </div>
</template>

<script>
export default {
    name: 'DetailsComponent'
}
</script>

<style scoped>

.details-grid {
    margin-left: auto;
    margin-right: auto;

    display: grid;
    grid-template-columns: repeat(4, 1fr);
    column-gap: 0;

    max-width: 1000px;

    background: white;
    box-shadow: 0px 4px 20px rgba(0,0,0,0.1);
    border-radius: 10px;
}

.details-box {
    padding: 10px 35px;
    position: relative;
}

.box-border-left::after {
    content: '';
    display: block;
    position: absolute;

    left: 0;
    top: 25%;
    width: 1px;
    height: 50%;
    background-color: hsl(0,0%,90%);
}

h2 {
    font-weight: 500;
}

h5 {
    margin-bottom: 0;
    font-weight: 500;
    color: hsl(0,0%,57%);
    letter-spacing: 1px;
}

</style>