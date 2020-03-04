<template>
    <div class="country">
        <div>
          <img 
            class="country__picture"
            :src="require(`@/images/${image}`)"
            alt=""
          >
          <span class="country__picture-price">
            от {{price}} Р
          </span>
      </div>
      
      <div class="country__title">
        {{title}}
      </div>

      <div class="country__name">
        {{name}}
      </div>

      <div v-show="destinations" class="country__destinations">
        {{destinations}}
      </div>

      <div class="country__duration">
        {{duration}}
      </div>

      <div v-show="extra" class="country__extra">
        {{extra}}
      </div>      
    </div>
</template>

<script>
export default {
  name: 'Country',
  props: {
    image: String,
    price: String,
    title: String,
    name: String,
    destinations: String,
    duration: String,
    extra: String
  }
}
</script>