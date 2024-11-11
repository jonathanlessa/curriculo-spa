<template>
  <div id="app">
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/skills">Skills</router-link> |
      <router-link to="/hobbies">Hobbies</router-link>
    </nav>
    <router-view/>
  </div>
</template>

<style>
  * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
  }

  nav {
    padding: 30px;
  }

  nav a {
    font-weight: bold;
    color: #2c3e50;
  }

  nav a.router-link-exact-active {
    color: #42b983;
  }

  body {
      font-family: 'Arial', sans-serif;
      background-color: #121212;
      color: #f0f0f0;
      margin: 0;
      padding: 0;
  }

  #app {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    text-align: center;
  }

  .section {
      margin-bottom: 20px;
      padding: 20px;
      border-radius: 10px;
      background-color: #1f1f1f;
      box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.4);
      transition: background-color 0.3s;
  }

  .section:hover {
      background-color: #292929;
  }

  .section h2 {
      color: #00adb5;
      font-size: 1.8em;
      margin-bottom: 10px;
      font-weight: bold;
      text-align: center;
  }

  .section p, .section ul {
      font-size: 1.1em;
      line-height: 1.6;
      color: #e0e0e0;
      text-align: justify;
  }

  .section ul {
      margin-top: 10px;
      padding-left: 20px;
  }

  .section ul li {
      margin-bottom: 8px;
      list-style-type: disc;
      text-align: left;
  }

  footer {
      background-color: #1f1f1f;
      color: #f0f0f0;
      padding: 20px;
      text-align: center;
      border-top: 1px solid #292929;
      box-shadow: 0 -3px 6px rgba(0, 0, 0, 0.3);
  }

  footer p {
      font-size: 1em;
      color: #e0e0e0;
      margin: 10px 0;
  }

  footer .social-icons {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin-top: 10px;
  }

  footer .social-icons a {
      color: #00adb5;
      transition: color 0.3s;
  }

  footer .social-icons a:hover {
      color: #00f2f2;
  }

  footer .social-icons i {
      font-size: 1.8em;
  }

  /* Responsividade para telas menores */
  @media (max-width: 768px) {
      .section h2 {
          font-size: 1.6em;
      }

      .section p, .section ul {
          font-size: 1em;
      }

      footer .social-icons i {
          font-size: 1.5em;
      }
  }
  header {
    text-align: center;
    margin: 20px 0;
  }
  .profile-pic {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      border: 4px solid #00adb5;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  }
</style>
