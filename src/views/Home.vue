<template>
  <div class="home">
    home
    <p>my name is {{ name }} and my age is {{ age }}</p>
    <button @click="handleClick">click me</button>
  </div>
</template>

<script>
export default {
  name: "Home",
  setup() {
    console.log("setup");

    let name = "mario";
    let age = 30;

    const handleClick = () => {
      console.log("youclickedme");
    };

    return { name, age, handleClick };
  },
};
</script>
