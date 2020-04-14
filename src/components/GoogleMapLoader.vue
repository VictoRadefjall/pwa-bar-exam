<template>
  <div>
    <div class="google-map columns" ref="googleMap"></div>
    <template v-if="Boolean(this.google) && Boolean(this.map)">
      <slot
        :google="google"
        :map="map"
      />
    </template>
  </div>
</template>