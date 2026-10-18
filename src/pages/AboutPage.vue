
<template>
  <f7-page name="about">
    <f7-navbar
      title="Про TaskFlow"
      back-link="Назад"
    />

    <div class="app-content">
      <div class="welcome-block">
        <h1>Про TaskFlow</h1>
        <p>
          TaskFlow — це PWA-застосунок для
          керування завданнями та відстеження
          їх виконання.
        </p>
      </div>

      <div class="info-card">
        <h2>Використані технології</h2>

        <ul>
          <li>Vue 3 — створення інтерфейсу</li>
          <li>Framework7 — мобільні компоненти</li>
          <li>Vite — збірка проєкту</li>
          <li>PWA — можливість встановлення застосунку</li>
        </ul>
      </div>

      <f7-button
        fill
        large
        href="/"
        class="about-button"
      >
        На головну
      </f7-button>
    </div>
  </f7-page>
</template>

<style scoped>
.info-card {
  background: #ffffff;
  padding: 20px;
  border-radius: 16px;
  border: 1px solid #e5eaf2;
}

.info-card h2 {
  margin: 0 0 16px;
  font-size: 20px;
  color: #172033;
}

.info-card ul {
  padding-left: 20px;
  margin: 0;
  color: #475569;
  line-height: 2;
}
</style>
