<style>
  /* Animation Keyframes */
  @keyframes fadeInUp {
    0% {
      opacity: 0;
      transform: translateY(20px);
    }
    100% {
      opacity: 1;
      transform: translateY(0);
    }
  }

  /* Apply Animation to the Text */
  .fade-in-up {
    animation: fadeInUp 0.3s ease-out;
    opacity: 0;
    animation-fill-mode: forwards;
  }

  /* Delay each element slightly for a cascading effect */
  .fade-in-up:nth-child(1) {
    animation-delay: 0.3s;
  }
  .fade-in-up:nth-child(2) {
    animation-delay: 0.6s;
  }
  .fade-in-up:nth-child(3) {
    animation-delay: 0.9s;
  }
</style>

<div style="position: relative; min-height: 100vh; padding: 20px; overflow: hidden;">
  <!-- Background Video -->
  <video autoplay muted loop style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: cover; z-index: -1;">
    <source src="EMF portfolio video.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>

  <!-- Overlay Content -->
  <div class="flex flex-col items-center justify-center p-6" style="position: relative; z-index: 1;">
    <!-- Text Section -->
    <div class="text-center mt-10 lg:mt-60">
      <h3 class="text-2xl lg:text-4xl font-regular text-white mb-2 lg:mb-4 fade-in-up">
        You're a real one! Welcome to
      </h3>
      <div class="mb-4 lg:mb-6 fade-in-up">
        <img src="EMF white logo.png" alt="EMF Logo">
      </div>

      <div class="overflow-hidden">
        <h3 class="text-xl lg:text-3xl font-regular text-white mb-2 lg:mb-4 text-info fade-in-up">
          Just your regular BSIT student from Gordon College Olongapo
        </h3>
      </div>
    </div>
  </div>
</div>
