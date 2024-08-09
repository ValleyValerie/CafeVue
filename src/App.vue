<script setup>
import Button from './components/Button.vue'
import NavBar from './components/NavBar.vue'
import Artist from './components/Artist.vue'

</script>

<template>
  <header >
    <NavBar  />
  </header>

  <section class=" sm:py-2 lg:py-8 " id="home">
        <div class="px-4 mx-auto max-w-7xl sm:px-6 lg:px-9">
            <div class="grid items-center grid-cols-1 gap-12 lg:grid-cols-2">
                <div>
                    <h1 class="mt-4 text-5xl font-medium lg:mt-8 sm:text-7xl xl:text-9xl animate__animated animate__slideInLeft ">Coffee<br> <i class="font-medium">Meets</i><br> Creativity</h1>
                    <p class="mt-4 text-lg lg:mt-8 sm:text-3xl animate__animated animate__slideInLeft ">Immerse yourself in a space where flavors blend and creativity thrives.</p> 
                </div>

                <div>
                    <img class=" sm:w-2/5 md:w-4/5 animate__animated animate__slideInRight " src="./assets/images/croissant_1.png" alt="croissants" />
                </div>
                <Button class="animate__animated animate__slideInLeft m-1 sm:text-xl lg:text-2xl "/>
                
            </div>
            <div class="relative  animate__animated animate__slideInRight h-20  ">
  <p class="absolute right-0 sm:text-lg lg:text-xl">REVIEWS: <br> 10/10</p>
</div>
        </div>
        
    </section>
 

  <section class="bg-white pt-8 pb-20" id="about">
    <div class="relative p-3">
      <div class="absolute top-0 left-0 ml-10 tracking-tighter">
        <h2 class="lg:text-7xl md:text-5xl font-medium"><i class="font-medium">We believe</i> <br> in the power</h2>
        <p class="lg:text-3xl font-medium italic mt-4">(25 years of <br> experience)</p>
        <p class="lg:text-xl mt-8 lg:max-w-sm ">
          Where every cup of coffee is brewed with passion and every bite of our artisanal baked goods is crafted with precision. <br><br> Our café is designed with a rustic charm, featuring reclaimed wood furnishings, soft, ambient lighting, and an open kitchen where guests can watch our artisans at work. The walls are adorned with local art, fostering a connection with the community and inspiring creativity.
        </p>
        
        <Button class=" mt-5 sm:text-xl lg:text-2xl "/> 
      </div>
      <div class="absolute top-0 right-0 mt-28 mr-48   text-right tracking-tighter">
        <h2 class="lg:text-7xl md:text-5xl font-medium">of great <br> <i class="font-medium">coffee</i></h2>
      </div>
      <div class="absolute bottom-0 right-0  mr-16   text-right tracking-tighter">
        <h2 class="lg:text-7xl md:text-5xl font-medium">and fresh <br> pastries.</h2>
      </div>
      <div class="flex justify-center mt-32  ">
        <img src="./assets/images/cupcake_1.png" alt="Cupcakes" class="object-cover  w-2/3 lg:w-2/5 md:w-2/6 animate__animated animate__fadeInUp ">
      </div>
      <div class="absolute top-0 right-0 mt-7 mr-10 text-right tracking-tighter">
        <p class=" right-0 sm:text-lg lg:text-xl">HOSPITALITY: <br> 10/10</p>
      </div>
      <div class="absolute  left-0 right-0 flex justify-center  ">
      <p class="text-center sm:text-lg lg:text-xl mt-5">COSINESS: <br> 10/10</p>
    </div>
    </div>
   
  
  </section>
  <section class="sm:py-2 lg:py-14 " id="menu">
    <h2 class="text-center lg:text-7xl md:text-5xl mb-7">Grab A Bite</h2>
      <div class="flex flex-wrap justify-center space-x-10 relative">
        <!-- Almond Bliss Croissant -->
        <div class="relative max-w-xs mb-10 flex flex-col">
          <img src="./assets/images/croissant_2.png" alt="Almond Bliss Croissant" class="rounded-full w-full mt-4 animate__animated animate__fadeInUp">
          <div class="text-left bg-opacity-75 p-2 animate__animated animate__fadeIn">
            <h3 class="lg:text-5xl md:text-3xl font-medium">Almond <i>Bliss</i> Croissant</h3>
            <p class="text-sm">This exquisite croissant is generously filled with a smooth almond cream, topped with slivered almonds.</p>
          </div>
        </div>
        <!-- Raspberry Jam Tart -->
        <div class="relative max-w-xs mb-10 flex flex-col">
          <img src="./assets/images/raspberry_jam_tart_1.png" alt="Lavender Honey Scones" class="rounded-full w-full mt-4 animate__animated animate__fadeInUp">
          <div class="text-center  bg-opacity-75 p-2 animate__animated animate__fadeIn">
            <h3 class="lg:text-5xl md:text-3xl font-medium">Raspberry <i>Delight Jam</i> Tart</h3>
            <p class="text-sm"> A flaky, buttery crust filled with a vibrant and tangy raspberry jam, perfectly balanced between sweetness and tartness.</p>
          </div>
        </div>
        <!-- Cheesecake -->
        <div class="relative max-w-xs mb-10 flex flex-col">
          <img src="./assets/images/chessecake_1.png" alt="Spiced Pumpkin Muffins" class="rounded-full w-full mt-4 animate__animated animate__fadeInUp">
          <div class="text-center  bg-opacity-75 p-2 animate__animated animate__fadeIn">
            <h3 class="lg:text-5xl md:text-3xl font-medium">Decadent <i>New York</i> Cheesecake</h3>
            <p class="text-sm"> A velvety smooth cheesecake with a rich, creamy texture and a buttery graham cracker crust, topped with a hint of vanilla.</p>
          </div>
        </div>
        <!-- Match Cake -->
        <div class="relative max-w-xs mb-10 flex flex-col">
          <img src="./assets/images/match_cake_1 (2).png" alt="Almond Bliss Croissant" class="rounded-full w-full mt-4 animate__animated animate__fadeInUp">
          <div class="text-left bg-opacity-75 p-2 animate__animated animate__fadeIn">
            <h3 class="lg:text-5xl md:text-3xl font-medium">Elegant <i>Matcha </i> Cake</h3>
            <p class="text-sm"> A light and airy cake infused with premium matcha, offering a delicate balance of earthy green tea flavors and subtle sweetness.</p>
          </div>
        </div>
        <!-- Macaroons -->
        <div class="relative max-w-xs mb-10 flex flex-col">
          <img src="./assets/images/macaroons_1.png" alt="Lavender Honey Scones" class="rounded-full w-full mt-4 animate__animated animate__fadeInUp">
          <div class="text-center  bg-opacity-75 p-2 animate__animated animate__fadeIn">
            <h3 class="lg:text-5xl md:text-3xl font-medium">Assorted <i>French</i> Macarons</h3>
            <p class="text-sm">A selection of delicate, crisp shells filled with luxurious ganache, buttercream, and jam in a variety of delectable flavors.</p>
          </div>
        </div>
        <!-- Spring_rolls -->
        <div class="relative max-w-xs mb-10 flex flex-col">
          <img src="./assets/images/Spring_rolls_1.png" alt="Spiced Pumpkin Muffins" class="rounded-full w-full mt-4 animate__animated animate__fadeInUp">
          <div class="text-center  bg-opacity-75 p-2 animate__animated animate__fadeIn">
            <h3 class="lg:text-5xl md:text-3xl font-medium">Vietnamese <i>Spring</i> Rolls</h3>
            <p class="text-sm"> Crisp vegetables, fresh herbs, and tender shrimp or tofu wrapped in rice paper, served with a savory peanut dipping sauce.</p>
          </div>
        </div>
      </div>
    </section>
    <section class= "bg-white pt-0" id="location">
      <img src="./assets/images/tart_1.png" class="mx-auto animate__animated animate__fadeIn" alt="Description of image">
      <h1 class="text-5xl font-medium mb-2 text-center animate__animated animate__fadeInUp">Come Visit Us</h1>
      <div class="flex justify-center items-center p-9 animate__animated animate__fadeInUp">
    <div class="grid grid-cols-2 gap-2">
      <div class="p-2 border text-center">New York City, NY</div>
      <div class="p-2 border text-center">123 Fifth Avenue, New York, NY 10011</div>
      <div class="p-2 border text-center">Los Angeles, CA</div>
      <div class="p-2 border text-center">456 Sunset Boulevard, Los Angeles, CA 90028</div>
      <div class="p-2 border text-center">Chicago, IL</div>
      <div class="p-2 border text-center">789 Michigan Avenue, Chicago, IL 60611</div>
      <div class="p-2 border text-center">Houston, TX</div>
      <div class="p-2 border text-center">101 Main Street, Houston, TX 77002</div>
      <div class="p-2 border text-center">Miami, FL</div>
      <div class="p-2 border text-center">202 Ocean Drive, Miami, FL 33139</div>
    </div>
  </div>
  <Artist />
    </section>
    

</template>

<style scoped>

</style>