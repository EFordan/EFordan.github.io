<script>
    import "../app.css";
    export const prerender = true;
    let menuOpen = false;
  </script>
  
  <svelte:head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100..900;1,100..900&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
  </svelte:head>
  
  <slot></slot>
  
  <nav class="bg-orange-400 p-4 fixed w-full top-0 z-50">
    <div class="container mx-auto flex flex-col items-center">
      <div class="mb-2">
        <img src="emf logo black.png" alt="EMF Portfolio Logo" class="h-8"> <!-- Adjust the height as needed -->
      </div>
  
      <!-- Navigation Link -->
      <div class="space-x-4 hidden lg:flex">
        <a href="/" class="text-black hover:bg-orange-300 focus:ring-4 focus:ring-orange-400 font-semibold rounded-lg px-4 py-2 transition duration-200">Home</a>
        <a href="/about" class="text-black hover:bg-orange-300 focus:ring-4 focus:ring-orange-400 font-semibold rounded-lg px-4 py-2 transition duration-200">About EMF</a>
        <a href="/portfolio" class="text-black hover:bg-orange-300 focus:ring-4 focus:ring-orange-400 font-semibold rounded-lg px-4 py-2 transition duration-200">Projects</a>
        <a href="/contact" class="text-black hover:bg-orange-300 focus:ring-4 focus:ring-orange-400 font-semibold rounded-lg px-4 py-2 transition duration-200">Contact</a>
      </div>

      <div class="lg:hidden mt-2">
        <button on:click={() => (menuOpen = !menuOpen)} class="text-black focus:outline-none">
          <!-- Icon for the hamburger menu -->
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>
  </nav>
  