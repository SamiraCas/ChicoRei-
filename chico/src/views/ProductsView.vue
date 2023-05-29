<script setup>
import { faker } from '@faker-js/faker';

const products = []

for (let index = 0; index < 21; index++) {
  const name = faker.commerce.product()
  const image = faker.image.urlPicsumPhotos()
  const price = faker.commerce.price({ max: 100, symbol: 'R$', dec: 0 })
  const description = faker.commerce.productDescription()

  const product = {
    name,
    image,
    price,
    description
  }

  products.push(product)
}

</script>


<template>
 
</style>