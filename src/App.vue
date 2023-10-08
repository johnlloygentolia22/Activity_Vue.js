<script setup>
import { ref } from 'vue';

const inputText = ref('hello')
const foods = ref('')

</script>
<template>
  
  <div  class="p-3 mb-2 bg-dark text-white">
    <div class="mx-auto p-2" style="width: 400px; ">
 <h2>   Select Recipe</h2>
    <select v-model="foods" class="form-select" aria-label="Default select example">
        <option value="1">Adobo</option>
        <option value="2">Chicken Mustard</option>
        <option value="3">kaldereta</option>
        <option value="4">Spaghetti</option>
        <option value="5">Beef Stick</option>
        <option value="6">Lompinang shanghai</option>
        
        
    </select>
    <div class="p-3 mb-2 bg-secondary text-white">
    <p v-if=" foods == '1'">
      <h1>Adobo</h1>
    <h5>Ingredients:</h5>
    <h5>500 grams of Chicken or Pork</h5>
    <h5>1/2 cup Soy Sauce</h5>
    <h5>1/4 cup Vinegar</h5>
    <h5>4 cloves of Garlic (minced)</h5>
    <h5>2 Bay Leaves</h5>
    <h5>1 teaspoon Black Peppercorns</h5>
    </p>
    <p v-if=" foods == '2'">
      <h1>Chicken Mustard</h1>
    <h5>Ingredients:</h5>
    <h5>4 Chicken Breasts (about 600 grams)</h5>
    <h5>1/4 cup Mustard Sauce</h5>
    <h5>1 Onion (chopped)</h5>
    <h5>4 cloves of Garlic (minced)</h5>
    <h5>2 tablespoons Butter</h5>
    <h5>1/2 cup Heavy Cream</h5>
    
    </p>
    <p v-if=" foods == '3'">
      <h1>Kaldereta</h1>
    <h5>Ingredients:</h5>
    <h5>1 pound Beef or Goat Meat (cubed)</h5>
    <h5>2 Potatoes (peeled and cubed)</h5>
    <h5>2 Carrots (peeled and sliced)</h5>
    <h5>1 Red Bell Pepper (sliced)</h5>
    <h5>1 cup Tomato Sauce</h5>
    <h5>2 tablespoons Liver Spread</h5>

    </p>
    <p v-if=" foods == '4'">
      <h1>Spaghetti</h1>
    <h5>Ingredients:</h5>
    <h5>8 ounces Spaghetti Noodles</h5>
    <h5>1/2 pound Ground Beef</h5>
    <h5>1 cup Tomato Sauce</h5>
    <h5>1 Onion (chopped)</h5>
    <h5>2 cloves of Garlic (minced)</h5>
    <h5>1/2 cup grated Cheese</h5>

    </p>
    <p v-if=" foods == '5'">
      <h1>Beef Stick</h1>
    <h5>Ingredients:</h5>
    <h5>1 pound Beef Strips (thinly sliced)</h5>
    <h5>1/4 cup Soy Sauce</h5>
    <h5>3 cloves of Garlic (minced)</h5>
    <h5>1 Onion (chopped)</h5>
    <h5>Wooden Skewers (soaked in water)</h5>
    <h5>Cooking Oil (for grilling or frying)</h5>

    
    </p>
    <p v-if=" foods == '6'">
      <h1>Lumpiang Shanghai</h1>
    <h5>Ingredients:</h5>
    <h5>1/2 pound Ground Pork</h5>
    <h5>1/4 cup Shrimp (minced)</h5>
    <h5>3 cloves of Garlic (minced)</h5>
    <h5>1 Onion (chopped)</h5>
    <h5>1 Carrot (grated)</h5>
    <h5>Lumpia (Spring Roll) Wrappers</h5>
    
    </p>

    <!-- <p v-else>3</p> -->
  </div>
  </div>
</div>
</template>