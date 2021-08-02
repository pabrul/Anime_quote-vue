<template>
  <header>
    <h1>{{ title }}</h1>
    <img alt="Saitama Meme" :src="'/assets/saitama.png'">

  </header>
</template>

<script>
export default {
  props: ["title"],
};
</script>

<style lang="scss" scoped>
header {
  padding: 24px 32px;
  display: flex;
  justify-content: center;
  flex-direction: row;
  flex-wrap: nowrap;
  align-content: center;
  align-items: flex-end;
  h1 {
    font-size: 2em;
    color: var(--dark);
    font-weight: 700;
    text-align: center;
    text-transform: uppercase;
    padding-bottom: 8px;
    border-bottom: 5px solid var(--primary);
  }
  
  img{
    width: 13%;
    margin-bottom: 0px;
    border-bottom: 5px solid var(--primary);
    margin-left: -16px;
    transition: all 1s linear;
    &:hover{
    opacity: 0.2;
    transition: 1s ease;
    }
    @media screen and (max-width: 768px) {
      width: 40%;
    }
  }
}
</style>
