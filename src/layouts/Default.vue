<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title>SDA-Video</v-toolbar-title>
      <v-text-field placeholder="search" class="ml-8"
        outlined rounded dense hide-details style="max-width:350px;"
        prepend-inner-icon="mdi-magnify"
      />
      <g-link class="nav__link" to="/">HoWe will build a virtual events platform using the Vue.js static site generator, Gridsome and Strapi.js for our backendme</g-link>
        <g-link class="nav__link" to="/about/">About</g-link>

            <v-spacer/>
      <v-btn>Create Event</v-btn>
    </v-app-bar>
    <!-- <header class="header">
      <strong>
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
        <p>{{ $static.metadata.siteDescription}}</p>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about/">About</g-link>
      </nav>
    </header> -->
    <v-main>
          <slot/> 

    </v-main>
  </v-app>
</template>

<static-query>
query {
  metadata {
    siteName,
    siteDescription
  }
}
</static-query>
