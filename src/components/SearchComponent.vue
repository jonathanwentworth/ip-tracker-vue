<template>
  <div class="search-wrapper">
    <h1>IP Address Tracker</h1>

    <div class="search">
        <input class="search-input" type="text" placeholder="Search for any IP address or domain">
        <button class="search-submit" type="submit">
            <img src="../assets/icon-arrow.svg" alt="">
        </button>
    </div>
    
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

  </div>
</template>

<script>
export default {
    name: 'DetailsComponent'
}
</script>

<style scoped>

.search-wrapper {
    background-image: url('../assets/pattern-bg.png');
    background-size: cover;
    background-position: center;

    text-align: center;
    color: white;

    padding: 30px;
    padding-bottom: 0;
}

.search {
    width: 100%;

    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}

.search-input {
    padding: 15px 20px;
    font-size: 18px;

    border-radius: 10px 0px 0px 10px;
    border: none;
    outline: none;

    width: 100%;
    max-width: 500px;
}

.search-input::placeholder {
    color: #999;
}

.search-submit {
    padding: 18px;

    border-radius: 0px 10px 10px 0px;
    border: none;
    outline: none;

    background: hsl(0, 0%, 17%);
    color: white;

    transition: all 0.2s ease-in-out;
}

.search-submit:hover {
    background: hsl(0, 0%, 25%);
    cursor: pointer;

    transition: all 0.2s ease-in-out;
}

.details-grid {
    margin-left: auto;
    margin-right: auto;

    display: grid;
    grid-template-columns: repeat(4, 1fr);
    column-gap: 0;

    width: 100%;
    max-width: 1000px;

    background: white;
    box-shadow: 0px 4px 20px rgba(0,0,0,0.1);
    border-radius: 10px;

    color: hsl(0,0%,17%);

    transform: translateY(50%);
    z-index: 999;
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