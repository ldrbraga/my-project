<template>
  <main class="root">
    <section class="heading">
      <div class="heading__title">
        <h1>{{ title }}</h1>
        <h2>{{ subtitle }}</h2>
      </div>
      <div>
        <nav>
          <ul class="social__list">
            <li class="social__list__item">
              <a class="social__list__item__link" href="https://twitter.com/ldrbraga" target="_blank">Twitter</a>
            </li>
            <li class="social__list__item">
              <a class="social__list__item__link" href="https://github.com/ldrbraga" target="_blank">Github</a>
            </li>
            <li class="social__list__item">
              <a class="social__list__item__link" href="https://codepen.io/ldrbraga/" target="_blank">Codepen</a>
            </li>
          </ul>
        </nav>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  data() {
    return {
      title: "Leandro Braga",
      subtitle: "Front End Developer."
    };
  }
};
</script>

<style lang="scss">
.root {
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.heading {
  &__title {
    display: flex;
    flex-direction: column;

    h1 {
      font-size: 70px;
      color: #fff;
      font-weight: 400;
    }

    h2 {
      font-size: 30px;
      color: #8e8e8e;
      font-weight: 300;
    }
  }
}
.social__list {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  padding: 0;
  max-width: 320px;
  padding: 30px 0;

  &__item {
    list-style: none;

    &__link {
      text-decoration: none;
    }
  }
}
</style>



