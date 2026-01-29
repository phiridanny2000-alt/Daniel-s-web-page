<div class="logo-container">
  <img src="logo.png" class="logo-main">
  <img src="orbit.png" class="orbit">
</div>
.logo-container {
  position: relative;
  width: 300px;
  margin: auto;
}

/* Main logo */
.logo-main {
  width: 100%;
  animation: pulse 3s infinite ease-in-out,
             rotateSlow 12s linear infinite;
}

/* Orbit ring */
.orbit {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  animation: spin 4s linear infinite;
}

/* Animations */
@keyframes spin {
  from { transform: rotate(0deg); }
  to   { transform: rotate(360deg); }
}

@keyframes pulse {
  0% { filter: drop-shadow(0 0 5px #00aaff); }
  50% { filter: drop-shadow(0 0 18px #00ccff); }
  100% { filter: drop-shadow(0 0 5px #00aaff); }
}

@keyframes rotateSlow {
  from { transform: rotate(0deg); }
  to   { transform: rotate(360deg); }
}
