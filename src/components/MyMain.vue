<template>
  <main>
    <div class="contents">
      <div class="container90">
        <div class="content">
          Contents goes here
        </div>
      </div>
    </div>

    <div class="bonus">
      <div class="container90">
        Sezione bonus
      </div>
    </div>
  </main>
</template>

<script>
export default {
    name: 'MyMain'
}
</script>

<style scoped lang="scss">
  .contents {
    height: 100px;
    background-color: black;
    color: white;
    display: flex;
    align-items: center;

    .content {
    color: white;
    }
    
  }

  .bonus {
    height: 100px;
    background-color: #0282F9;
    display: flex;
    align-items: center;
  }


  

</style>