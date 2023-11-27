<script setup lang="ts">
import Registration from '../components/RegistrationTemplate.vue'
import RegistrationInfo from '../components/RegistrationInfo.vue'
</script>

<template>
  <section class="home-cntr">
    <div class="section-panel info-panel">
      <div class="section-header">
        <img
          class="logo"
          src="https://assets-global.website-files.com/629921453332210f9bc4b034/653018270442aa9a099ead01_prezent-logo.svg"
          alt="logo"
        />
      </div>
      <RegistrationInfo />
    </div>

    <div class="section-panel form-panel">
      <div class="section-header">
        <img
          class="resp-logo"
          src="https://assets-global.website-files.com/629921453332210f9bc4b034/653018270442aa9a099ead01_prezent-logo.svg"
          alt="logo"
        />
      </div>
      <Registration />
    </div>
  </section>
</template>

<style scoped>
.home-cntr {
  display: flex;
}

.section-header {
  height: 10svh;
  display: flex;
  align-items: center;
}

.section-header img {
  width: 120px;
}

.resp-logo {
  display: none;
}

.info-panel {
  padding: 1rem 5% 1rem 8%;
  width: 55%;
}

.form-panel {
  background-color: #1075ab;
  padding: 1rem 8% 1rem 5%;
  width: 45%;
}

@media (max-width: 1280px) {
  .section-panel {
    padding: 2rem;
  }
}

@media (max-width: 768px) {
  section {
    flex-direction: column-reverse;
  }

  .section-panel {
    width: 100%;
  }

  .info-panel {
    padding: 0 2rem 2rem 2rem;
  }

  .info-panel .section-header {
    display: none;
  }

  .logo {
    display: none;
  }
  .resp-logo {
    display: block;
  }

  .form-panel {
    background-color: white;
    padding: 1rem 2rem;
  }
}
</style>
