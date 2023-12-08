<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footer-section">
        <h3>Bellu Clients</h3>
        <ul>
          <li><a href="#">Contact Us</a></li>
          <li><a href="#">FAQ</a></li>
          <li><a href="#">Bellu University</a></li>
        </ul>
      </div>
      <div class="footer-logo">
        <img src="./pictures/img.png" alt="Bellu Logo" width="50" height="50" />
      </div>
      <div class="footer-section">
        <h3>For Salons</h3>
        <ul>
          <li><a href="#">Bellu Labs</a></li>
          <li><a href="#">Salon Partnerships</a></li>
          <li><a href="#">Technical Support</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      <p>© Bellu LLC - 2023</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style>
.footer {
  background-color: #333;
  color: white;
  text-align: center;
  padding: 20px 0;
}

.footer-content {
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.footer-section h3 {
  margin-bottom: 10px;
}

.footer-section ul {
  list-style: none;
  padding: 0;
}

.footer-section ul li a {
  color: white;
  text-decoration: none;
  display: block;
  margin-bottom: 5px;
}

.footer-logo {
  text-align: center;
}

.footer-bottom {
  margin-top: 20px;
}

.footer-section h3 {
  margin-bottom: 10px;
  text-decoration: underline; /* Add underline */
}

/* Responsive adjustments */
@media (max-width: 600px) {
  .footer-content {
    flex-direction: column;
  }
}
</style>
