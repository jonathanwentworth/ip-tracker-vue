<template>
  <div class="search-wrapper">
    <h1>IP Address Tracker</h1>

    <div class="search">
        <input class="search-input" type="text" placeholder="Search for any IP address or domain">
        <button class="search-submit" type="submit">
            <img src="../assets/icon-arrow.svg" alt="">
        </button>
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
    width: 100vw;
    background-image: url('../assets/pattern-bg.png');
    background-size: cover;
    background-position: center;

    text-align: center;
    color: white;

    padding: 30px;
    padding-bottom: 120px;
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

</style>