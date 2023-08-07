<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
  body {
    margin: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    background-color: #111;
  }

  .container {
    position: relative;
    width: 80vw;
    max-width: 300px;
    height: auto;
  }

  .monkey-img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    opacity: 0;
    transition: opacity 1s ease-in-out;
  }

  .text {
    color: #f4f4f4;
    font-size: 18px;
    font-weight: bold;
    text-transform: uppercase;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 2;
    transition: opacity 1s ease-in-out;
  }

  .container:hover .text {
    opacity: 0;
  }

  .container:hover .monkey-img {
    opacity: 1;
  }
</style>
</head>
<body>
  <div class="container">
    <img class="monkey-img" src="https://www.npr.org/sections/thetwo-way/2017/09/12/550417823/-animal-rights-advocates-photographer-compromise-over-ownership-of-monkey-selfie-image.png" alt="Monkey">
    <div class="text">SHA</div>
  </div>
</body>
</html>
