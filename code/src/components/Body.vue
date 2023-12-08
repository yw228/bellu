<template>
  <div class="body">
  <div class="person-section">
    <h1>PERSONALIZED PRODUCTS FOR HEALTHY HAIR</h1>
    <button @click="findProducts">Find My Products</button>
  </div>

  <div class="quiz-section">
      <div class="quiz-image">
      </div>
      <div class="quiz-content">
        <h2>Have you ever wondered which shampoo and conditioner are best for your hair?</h2>
        <p>With the Bellu Product Finder Quiz, receive an in-depth analysis of your hair and which products are best for you.</p>
        <button @click="startQuiz">Bellu Hair Quiz</button>
      </div>
  </div>

  <div class="reviews-section">
      <h2>Client Reviews</h2>
      <div class="review-carousel">
        <button @click="prevReview" class="carousel-control left">&lt;</button>
        <div class="review-card" v-for="(review, index) in reviews" :key="index">
          <div class="review-image">
            <img :alt="review.altText">
          </div>
          <div class="review-content">
            <h3>Add a subheading</h3>
            <p>subheading</p>
          </div>
        </div>
        <button @click="nextReview" class="carousel-control right">&gt;</button>
      </div>
  </div>

    <div class="feature-section">
      <div class="feature-image">
      </div>
      <div class="feature-content">
        <h2>With a Bellu Hair Test, You Get:</h2>
        <ul class="feature-list">
          <li><span class="checkmark">✔</span>Microscopic Hair Analysis</li>
          <li><span class="checkmark">✔</span>Customized Product Routine</li>
          <li><span class="checkmark">✔</span>Personalized Hair and Lifestyle Tips</li>
          <li><span class="checkmark">✔</span>Elasticity, Moisture, and Root Health Ratings</li>
          <li><span class="checkmark">✔</span>Additional recommendations from analysts</li>
        </ul>
        <button @click="getStarted">Get Started</button>
      </div>
    </div>

  <div class="loyalty-section">
    <div class="loyalty-content">
      <h2>Loyal to You, Not Brands.</h2>
      <p>We have sifted through thousands of top-rated products for your hair needs.</p>
      <p>No matter if your hair is straight, curly, thin, oily, or dry – Bellu can give you a custom hair routine that will change your hair game.</p>
    </div>
    <div class="loyalty-image">
    </div>
  </div>

  <div class="social-media-section">
    <h1>we are #bellubeauty</h1>
    <p>Follow us on Social Media for more Hair Tips</p>
    <div class="social-icons">
      <a href="https://instagram.com" target="_blank"><img src="./icon/icons8-instagram-50.png" alt="Instagram" /></a>
      <a href="https://facebook.com" target="_blank"><img src="./icon/icons8-facebook-50.png" alt="Facebook" /></a>
      <a href="https://tiktok.com" target="_blank"><img src="./icon/icons8-tik-tok-50.png" alt="TikTok" /></a>
      <a href="https://youtube.com" target="_blank"><img src="./icon/icons8-youtube-50.png" alt="YouTube" /></a>
    </div>
  </div>
  </div>


</template>

<script>

export default {
  methods: {
    findProducts() {
      // Logic to find products
    },
    startQuiz() {
      // Logic to start the quiz
    },
    getStarted() {
      // Logic to 'Get Started'
    },
  }
}
</script>

<style>
.body,
.person-section,
.quiz-section,
.feature-section,
.loyalty-section,
.social-media-section {
  background-color: white; /* White background */
}

/* Set the text color of all content to black */
.body,
.body h1,
.body h2,
.body p,
.body button,
.body li {
  color: black; /* Black text */
}


.body {
  display: flex;
  flex-direction: column;
  height: 300vh; /* Set the height of the body to the full viewport height */
}

.body > div {
  flex: 1; /* Each direct child div will take up an equal amount of space */
  display: flex;
  flex-direction: column; /* Stack the content of each section vertically */
  justify-content: center; /* Center content vertically */
  align-items: center; /* Center content horizontally */
}

.person-section {
  background-image: url('@/components/pictures/Copy of First Picture with Gradient Home Page.jpg');
  background-size: cover;
  background-position: center;
  height: 100vh; /* Adjust height as needed */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.person-section h1 {
  color: grey;
  /* Additional styling for the headline */
}

.person-section button {
  background-color: white; /* Set the button background to white */
  color: grey; /* Set the button text color to grey */
  border: 1px solid grey; /* Set the border color to grey */
  border-radius: 25px; /* Gives the button rounded corners */
  padding: 10px 20px; /* Add padding inside the button */
  font-size: 16px; /* Set the font size */
  cursor: pointer; /* Changes the cursor to a pointer on hover */
  outline: none; /* Removes the outline to avoid the browser default focus style */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Optional: Adds a subtle shadow to the button */
  transition: all 0.3s ease; /* Optional: Adds a transition effect on hover */
}

.person-section button:hover {
  background-color: #f8f8f8; /* Slightly changes the button background on hover */
  /* Additional hover styles as needed */
}


.quiz-section {
  display: flex;
  align-content: center;
  justify-content: space-around;
  flex-direction: row;
}

.quiz-image {
  background-image: url('@/components/pictures/Copy of Premium Hair Test 1.jpg');
  background-size: cover;
  background-position:left;
  flex:2;
  min-width: 1000px; /* Adjust minimum width as needed */
  min-height: 500px; /* Adjust height as needed */
  padding-bottom: 500px;
}

.quiz-content {
  flex: 1; /* Adjust the flex value as needed */
  padding: 20px;
}

.quiz-content h2 {
  color: #333; /* Dark grey color for the text */
}

.quiz-content p {
  color: #333;
}

.quiz-content button {
  background-color: #333;
  color: white;
  border: none;
  padding: 20px 20px;
  border-radius: 20px;
  cursor: pointer;
  transition: background-color 0.3s ease;
  margin: 0 auto; /* Center the button horizontally */
  display: block; /* Ensure it takes up the full width of the container */
}
.quiz-section button:hover {
  background-color: #555; /* Slightly lighter grey on hover */
}


.feature-section {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 0 auto;
  max-width: 1200px; /* Adjust the max width as necessary */
}


.feature-content {
  flex-basis: 50%;
  padding: 20px;
  text-align: left; /* Align text to the left */
  display: flex; /* Use flexbox to align child elements */
  flex-direction: column; /* Stack children vertically */
  justify-content: center; /* Center children along the vertical line */
  align-items: center; /* Center children along the horizontal line */
}

.feature-list {
  list-style: none;
  padding: 0;
}
.feature-image {
  flex-basis: 50%;
  background-image: url('@/components/pictures/Copy of Standard Hair Test 1.png');
  background-size: cover;
  background-position: center;
  min-height: 400px; /* Adjust to your preference */
}

.feature-list li {
  margin-bottom: 10px;
  font-size: 1.2em; /* Adjust to your preference */
}

.checkmark {
  color: green; /* or any color you prefer */
  margin-right: 5px;
}

button {
  background-color: grey; /* Adjust to match your design */
  color: white; /* Set the text color to white */
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  font-size: 1.2em; /* Adjust to your preference */
  margin-top: 20px; /* Spacing above the button */
  align-self: center; /* Center the button inside the flex container */
}

button:hover {
  background-color: #555; /* Adjust to match your design */
}

.loyalty-section {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 20px;
  background: url('@/components/pictures/Copy of guy-598180_1280.jpg') no-repeat center center;
  background-size: cover;
  min-height: 500px; /* Adjust the height as needed */
}

.loyalty-content {
  flex-basis: 50%;
  padding: 20px;
}

.loyalty-content h2 {
  /* Additional styling for the header text */
  color: white; /* Dark grey color for the text */
  font-size: 80px; /* Size of icons, you might need to adjust if you're using font icons */
}

.loyalty-content p {
  /* Additional styling for the paragraphs */
  color: white;
  font-size: 30px; /* Size of icons, you might need to adjust if you're using font icons */
}

.reviews-section {
  text-align: center;
}

.review-carousel {
  display: flex;
  align-items: center;
  justify-content: center;
}

.review-card {
  margin: 0 10px;
  background-color: #f0f0f0;
  padding: 20px;
  border-radius: 10px;
  width: 200px; /* Adjust the width as needed */
}

.review-image img {
  border-radius: 50%;
  width: 100px; /* Adjust the size as needed */
  height: auto;
}

.carousel-control {
  background: none;
  border: none;
  font-size: 2em;
  cursor: pointer;
}


.social-media-section {
  text-align: center;
  background-color: #f9f9f9; /* or the color matching the image background */
  padding: 40px 0; /* Adjust padding to match design */
}

.social-media-section h2 {
  color: #333; /* Dark grey text color */
  font-weight: normal;
  text-transform: lowercase; /* Lowercase text as seen in the image */
  font-size: 24px; /* Adjust to match design */
  margin-bottom: 8px; /* Space between the title and subtitle */
}

.social-media-section p {
  color: #777; /* Light grey text color */
  margin-bottom: 24px; /* Space between the subtitle and icons */
}

.social-icons a {
  display: inline-block;
  margin: 0 10px; /* Space between icons */
  font-size: 24px; /* Size of icons, you might need to adjust if you're using font icons */
  opacity: 0.7; /* Icons appear slightly faded */
}

.social-icons a:hover {
  opacity: 1; /* Full opacity on hover */
}

.social-media-section h1 {
  font-size: 80px; /* Adjust the font size as needed */
  color: grey;
}

.social-media-section p {
  font-size: 40px; /* Adjust the font size as needed */
}

</style>
