<template>
  <div>
    <h1>Mon blog Nuxt 3 + Content 2</h1>
    <nav>
      <ul>
        <ContentNavigation v-slot="{ navigation }">
          <li v-for="link of navigation" :key="link._path" >
            <NuxtLink :to="link._path">
              {{ link.title }}
            </NuxtLink>
          </li>
        </ContentNavigation>
      </ul>
    </nav>
  </div>
</template>
