<template>
	<header class="header-style-two">

		<div id="sticky-header" class="menu-area sticky-menu">
			<div class="container custom-container">
				<div class="row">
					<div class="col-12">
						<div class="mobile-nav-toggler">
							<svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="bars" class="svg-inline--fa fa-bars fa-w-14" role="img" viewBox="0 0 448 512"><path fill="currentColor" d="M16 132h416c8.837 0 16-7.163 16-16V76c0-8.837-7.163-16-16-16H16C7.163 60 0 67.163 0 76v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16z"/></svg>
						</div>
						<div class="menu-wrap">

							<nav class="menu-nav show">
								<div class="logo">
									<nuxt-link to="/"><img src="/web/img/logo/logo.png" alt="Logo" class="zippk_logo"></nuxt-link>
								</div>
								<div class="navbar-wrap main-menu d-none d-lg-flex">
									<ul class="navigation">
										<li><nuxt-link to="/">Home</nuxt-link></li>
										<li><nuxt-link to="/movies">Movies</nuxt-link></li>
										<li><nuxt-link to="/seasons">Seasons</nuxt-link></li>
										<li><nuxt-link to="/animations">Animes</nuxt-link></li>
									</ul>
								</div>
								<div class="header-action d-none d-md-block">
									<ul>
										<li class="d-none d-xl-block">
											<div class="footer-search">
												<form action="#">
													<input type="text" placeholder="FIND FAVORITE MEDIA">
													<button>
														<svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="search" class="svg-inline--fa fa-search fa-w-16" role="img" viewBox="0 0 512 512"><path fill="currentColor" d="M505 442.7L405.3 343c-4.5-4.5-10.6-7-17-7H372c27.6-35.3 44-79.7 44-128C416 93.1 322.9 0 208 0S0 93.1 0 208s93.1 208 208 208c48.3 0 92.7-16.4 128-44v16.3c0 6.4 2.5 12.5 7 17l99.7 99.7c9.4 9.4 24.6 9.4 33.9 0l28.3-28.3c9.4-9.4 9.4-24.6.1-34zM208 336c-70.7 0-128-57.2-128-128 0-70.7 57.2-128 128-128 70.7 0 128 57.2 128 128 0 70.7-57.2 128-128 128z"/></svg>
													</button>
												</form>
											</div>
										</li>
									</ul>
								</div>
							</nav>
						</div>

						<!-- Mobile Menu  -->
						<!-- <div class="mobile-menu">
							<div class="close-btn"><i class="fas fa-times"></i></div>
							<nav class="menu-box">
								<div class="nav-logo"><a href="index.html"><img src="/web/img/logo/logo.png" alt="" title=""></a>
								</div>
								<div class="menu-outer">
									<ul class="navigation">
										<li class="active menu-item-has-children"><a href="#">Home</a>
											<div class="dropdown-btn"><span class="fas fa-angle-down"></span></div>
										</li>
										<li class="menu-item-has-children"><a href="#">Movie</a>
											<div class="dropdown-btn"><span class="fas fa-angle-down"></span></div>
										</li>
										<li><a href="tv-show.html">tv show</a></li>
										<li><a href="pricing.html">Pricing</a></li>
										<li class="menu-item-has-children"><a href="#">blog</a>
											<div class="dropdown-btn"><span class="fas fa-angle-down"></span></div>
										</li>
										<li><a href="contact.html">contacts</a></li>
									</ul>
								</div>
								<div class="social-links">
									<ul class="clearfix">
										<li><a href="#"><span class="fab fa-twitter"></span></a></li>
										<li><a href="#"><span class="fab fa-facebook-square"></span></a></li>
										<li><a href="#"><span class="fab fa-pinterest-p"></span></a></li>
										<li><a href="#"><span class="fab fa-instagram"></span></a></li>
										<li><a href="#"><span class="fab fa-youtube"></span></a></li>
									</ul>
								</div>
							</nav>
						</div> -->
						<div class="menu-backdrop"></div>
						<!-- End Mobile Menu -->
					</div>
				</div>
			</div>
		</div>

	</header>
</template>

<style>
	.header-style-two {position: relative;}
	.header-style-two .menu-area {background: #252631;padding: 8px 0;}
	.custom-container {max-width: 1420px;}
	.col-12 {
	    flex: 0 0 100%;
	    max-width: 100%;
	}
	.menu-area .mobile-nav-toggler {
	    position: relative;
	    float: right;
	    font-size: 30px;
	    cursor: pointer;
	    line-height: 1;
	    color: #fff;
	    display: none;
	    margin-top: 7px;
	}
	.menu-nav {
	    display: flex;
	    align-items: center;
	    flex-wrap: wrap;
	    justify-content: flex-start;
	}
	.navbar-wrap {
	    display: flex;
	    flex-grow: 1;
	}
	.navbar-wrap > ul {
	    display: flex;
	    flex-direction: row;
	    flex-wrap: wrap;
	    margin-left: auto;
	    margin-right: auto;
	}
	.navbar-wrap > ul > li {
	    display: block;
	    position: relative;
	}
	.navbar-wrap > ul > li > a {
	    font-size: 14px;
	    font-weight: 700;
	    text-transform: uppercase;
	    color: #f0f0f0;
	    padding: 38px 23px;
	    display: block;
	    line-height: 1;
	    position: relative;
	    z-index: 1;
	}
	.sticky-menu {
	    left: 0;
	    padding: 0 0;
	    margin: auto;
	    position: fixed;
	    top: 0;
	    width: 100%;
	    z-index: 99;
	    background: #171d22;
	    -webkit-animation: 1000ms ease-in-out 0s normal none 1 running fadeInDown;
	    animation: 1000ms ease-in-out 0s normal none 1 running fadeInDown;
	    -webkit-box-shadow: 0 10px 15px rgb(25 25 25 / 10%);
	    box-shadow: 0 10px 15px rgb(25 25 25 / 10%);
	    border-radius: 0;
	}
	.header-action > ul {
	    display: flex;
	    align-items: center;
	    margin-left: 10px;
	}
	.header-action > ul > li {
	    position: relative;
	    margin-left: 30px;
	}
	.header-action > ul > li:first-child {margin-left: 0;}
	.footer-search form {
	    min-width: 285px;
	    position: relative;
	    margin-left: 30px;
	}
	.header-style-two .header-action .footer-search form {margin-left: 0;}
	.header-style-two .menu-area.sticky-menu {padding: 0 0;}
	.menu-backdrop {
	    position: fixed;
	    right: 0;
	    top: 0;
	    width: 100%;
	    height: 100%;
	    z-index: 2;
	    transition: all 700ms ease;
	    -moz-transition: all 700ms ease;
	    -webkit-transition: all 700ms ease;
	    -ms-transition: all 700ms ease;
	    -o-transition: all 700ms ease;
	    opacity: 0;
	    visibility: hidden;
	    background: #171d22;
	}
</style>