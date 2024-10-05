<style>
    /* Background video styles */
  /* Background video styles */
  .background-video {
    position: fixed; /* Ensures the video is fixed and covers the whole viewport */
    top: 0;
    left: 0;
    width: 100vw; /* Full viewport width */
    height: 100vh; /* Full viewport height */
    object-fit: cover; /* Ensures the video scales properly to cover the area */
    z-index: -1; /* To make sure it's behind the content */
    opacity: 97%; /* Slight transparency */
  }
  
  /* Modify the existing container styles */
  .social-container {
    position: relative;
    z-index: 1; /* Ensures content appears above the video */
    height: 100vh; /* Ensures the content fills the whole screen */
    display: flex;
    flex-direction: column;
    justify-content: center; /* Vertically center the content */
    align-items: center; /* Horizontally center the content */
    padding: 20px;
  }
  
  /* Other existing styles */
  .social-icons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 20px;
    justify-content: center;
    align-items: center;
    padding: 0 15px;
  }
  
  .social-icons a {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: white;
    font-size: 0.9rem;
    font-weight: bold;
    text-decoration: none;
    transition: transform 0.3s ease, color 0.3s ease;
  }
  
  .social-icons a:hover {
    transform: scale(1.1);
    color: #ff9129;
  }
  
  .social-icons svg {
    width: 60px;
    height: 60px;
    fill: white;
  }
  
  .heading {
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: bold;
    color: white;
    font-size: 2rem;
    text-align: center;
    margin-bottom: 20px; /* Add some spacing below the heading */
  }
  
  @media (max-width: 768px) {
    .social-icons {
      grid-template-columns: repeat(2, 1fr);
    }
  
    .heading {
      font-size: 1.5rem;
    }
  
    .social-icons svg {
      width: 50px;
      height: 50px;
    }
  
    .social-icons a span {
      font-size: 0.8rem;
    }
  }
  
  @media (max-width: 480px) {
    .social-icons {
      grid-template-columns: 1fr;
    }
  
    .heading {
      font-size: 1.2rem;
    }
  
    .social-icons svg {
      width: 40px;
      height: 40px;
    }
  
    .social-icons a span {
      font-size: 0.7rem;
    }
  }
  
  </style>
  
  <div class="social-container">
    <!-- Background video -->
    <video class="background-video" autoplay muted loop>
      <source src="EMF contacts.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <div class="heading">
      <h1>For more details or inquiries, you can reach me out with one of these social medias! I'm honored to interact with you.</h1>
    </div>
  
    <div class="social-icons">
      <a href="https://www.youtube.com/@EMFordan" target="_blank" aria-label="YouTube">
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M23.498 6.186a2.946 2.946 0 0 0-2.073-2.078C19.6 3.5 12 3.5 12 3.5s-7.6 0-9.425.608A2.946 2.946 0 0 0 .5 6.186 30.6 30.6 0 0 0 0 12a30.6 30.6 0 0 0 .498 5.814 2.946 2.946 0 0 0 2.073 2.078C4.4 20.5 12 20.5 12 20.5s7.6 0 9.425-.608a2.946 2.946 0 0 0 2.073-2.078A30.6 30.6 0 0 0 24 12a30.6 30.6 0 0 0-.502-5.814zM9.75 15.42V8.579l6.369 3.421-6.369 3.42z"/>
        </svg>
        <span>YouTube</span>
      </a>
  
      <a href="https://www.behance.net/edwardfordan" target="_blank" aria-label="Behance">
        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24">
          <path d="M22.944 9.887h-6.674c.149-1.004 1.181-1.702 2.231-1.702 1.263 0 2.32.452 2.948 1.265h1.7c-.793-1.729-2.406-2.881-4.676-2.881-2.84 0-5.063 2.188-5.063 5.063s2.188 5.063 5.063 5.063c2.24 0 4.26-1.405 4.617-3.615h-3.964v-1.67h5.817c.061-.29.088-.594.088-.906 0-1.902-1.54-3.442-3.442-3.442zm-6.054 4.264c.238 1.008 1.172 1.741 2.316 1.741.893 0 1.801-.566 2.034-1.741h-4.35zm-16.89 5.406h9.69c3.182 0 4.648-1.993 4.648-4.148 0-1.628-.927-3.057-2.717-3.444 1.374-.529 1.991-1.654 1.991-2.961 0-2.035-1.529-4.045-4.835-4.045h-8.777v14.598zm7.405-12.258c1.648 0 2.384.859 2.384 2.005 0 1.186-.816 2.096-2.383 2.096h-4.31v-4.101h4.309zm-4.31 5.792h4.649c1.773 0 2.536.875 2.536 2.108 0 1.306-.963 2.165-2.618 2.165h-4.567v-4.273zm13.905-11.101h-5.02v1.563h5.02v-1.563z"/>
        </svg>
        <span>Behance</span>
      </a>
  
      <a href="https://www.facebook.com/EMFordan" target="_blank" aria-label="Facebook">
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M22.675 0H1.325C.593 0 0 .593 0 1.326v21.348C0 23.407.593 24 1.325 24H12.82v-9.294H9.692V10.62h3.128V8.413c0-3.1 1.892-4.788 4.657-4.788 1.325 0 2.463.099 2.797.143v3.24h-1.918c-1.505 0-1.796.715-1.796 1.763v2.31h3.587l-.467 3.086h-3.12V24h6.116c.73 0 1.324-.593 1.324-1.326V1.326C24 .593 23.407 0 22.675 0z"/>
        </svg>
        <span>Facebook</span>
      </a>
  
      <a href="https://twitter.com/EMFordan" target="_blank" aria-label="Twitter">
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M23.953 4.57a10.005 10.005 0 0 1-2.825.775 4.958 4.958 0 0 0 2.163-2.723 10.14 10.14 0 0 1-3.127 1.195 4.925 4.925 0 0 0-8.388 4.49A13.978 13.978 0 0 1 1.671 3.15a4.822 4.822 0 0 0-.666 2.475 4.92 4.92 0 0 0 2.188 4.096 4.9 4.9 0 0 1-2.23-.615v.061a4.923 4.923 0 0 0 3.946 4.827 4.934 4.934 0 0 1-2.224.084 4.927 4.927 0 0 0 4.604 3.42 9.874 9.874 0 0 1-6.102 2.104c-.395 0-.785-.023-1.17-.067a13.978 13.978 0 0 0 7.557 2.212c9.054 0 14.002-7.496 14.002-13.986 0-.21 0-.423-.015-.634A9.936 9.936 0 0 0 24 4.59a9.988 9.988 0 0 1-2.047 2.236z"/>
        </svg>
        <span>Twitter</span>
      </a>
      
    </div>
  
    <!-- Button to send Gmail -->
    <div class="flex justify-center mt-8">
      <a href="https://mail.google.com/mail/u/0/?view=cm&fs=1&to=202210106@gordoncollege.edu.ph" 
         target="_blank" 
         class="bg-orange-400 text-white font-bold py-2 px-4 rounded hover:bg-orange-700 transition">
        Want to send an E-mail? Click here
      </a>
    </div>
  </div>
  