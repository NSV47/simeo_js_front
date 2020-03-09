<template>
  <div>
     <h1>Мое приложение</h1>
    <nav>
      <ul>
        <li>
          <router-link to="/">Карта</router-link>
        </li>
        <li>
          <router-link to="/about">О проекте</router-link>
        </li>
      </ul>
    </nav>
    <router-view></router-view>
  </div>
</template>

<script>

export default {
  name: "Layout",
};
</script>
