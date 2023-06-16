<template>
    <div>
        <header>
            <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <nuxt-link to="/" class="nav-link">home</nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/about" class="nav-link">about us</nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/service" class="nav-link">our service</nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/contact" class="nav-link">contact us</nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/products" class="nav-link">products</nuxt-link>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
       
      </ul>
      <form class="d-flex">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
        </header>

        <main>
            <slot></slot>
        </main>

        <footer>
            <section>
              <div class="container">
                <div class="row">
                  <div class="col-md-3">
                    <img src="https://codeit.com.np/images/1642171339codeIT%20logo.png" alt="" height="60px">
                    <p>9862130505, 025-525163</p>
                    <p>info@codeit.com.np</p>
                    <p>prithivi path, dharan</p>
                  </div>
                  <div class="col-md-3">
                    <h1>Quick links</h1>
                    <p>About us</p>
                    <p>Contact link</p>
                    <p>Gallery</p>
                    <p>Blog</p>
                  </div>
                  <div class="col-md-3">
                    <h1>Bank Account Detail:</h1>
                    <p><b>Bank:</b>Nepal Bank Limited</p>
                    <p><b>Account Name:</b>CODE IT</p>
                    <p><b>Ac/No.:</b>01600106885462000001</p>
                    <p><b>branch:</b>Dharan</p>
                    <img src="https://codeit.com.np/asset/img/fonepay-bg.png" alt="" height="30px">
                    <img src="https://codeit.com.np/asset/img/codeit-qr.jpg" alt="" height="60px">
                  </div>
                  <div class="col-md-3">
                    <h1>Download App</h1>
                    <p>Download our mobile app</p>
                    <img src="https://codeit.com.np/mobile/appstore.png" alt="" height="40px">
                    <img src="https://codeit.com.np/mobile/googleplay.png" alt="" height="40px">
                  </div>
                </div>
              </div>
            </section>
        </footer>
    </div>
</template>