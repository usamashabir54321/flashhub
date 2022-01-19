<template>
	<main>
		<Nuxt keep-alive />
	</main>
</template>

<style name="common_css">
	*, ::after, ::before {
		margin: 0;
		padding: 0;
	    box-sizing: border-box;
	    outline: none;
	    text-decoration: none;
	}
	body {
		font-family: -webkit-pictograph;
		font-weight: 500;
		font-style: normal;
		font-size: 14px;
		color: #bcbcbc;
	}
	html::-webkit-scrollbar {width: 6px;}
	html::-webkit-scrollbar-thumb {
	    background: #434343;
	    box-shadow: inset 2px 2px 2px hsl(0deg 0% 100% / 25%), inset -2px -2px 2px rgb(0 0 0 / 25%);
	}
	html::-webkit-scrollbar-track {background: linear-gradient(90deg,#434343,#434343 1px,#111 0,#111);}
	main {background:black;}
	.img {max-width: 100%;transition: all 0.3s ease-out 0s;}
	a,.button {
		-webkit-transition: all 0.3s ease-out 0s;
		-moz-transition: all 0.3s ease-out 0s;
		-ms-transition: all 0.3s ease-out 0s;
		-o-transition: all 0.3s ease-out 0s;
		transition: all 0.3s ease-out 0s;
	}
	a:focus,.btn:focus,.button:focus {
		text-decoration: none;
		outline: none;
		box-shadow: none;
	}
	a:hover,.portfolio-cat a:hover,.footer -menu li a:hover {
		color: #2B96CC;
		text-decoration: none;
	}
	a,button {color: #1696e7;outline: medium none;}
	button:focus,input:focus,input:focus,textarea,textarea:focus{outline: 0}
	h1,h2,h3,h4,h5,h6 {
		font-family: -webkit-pictograph;
		color: #fff;
		margin-top: 0px;
		font-style: normal;
		font-weight: 700;
		text-transform: normal;
	}
	h1 a,h2 a,h3 a,h4 a,h5 a,h6 a {color: inherit;}
	h1 {font-size: 40px;font-weight: 500;}
	h2 {font-size: 35px;}h3 {font-size: 28px;}h4 {font-size: 22px;}h5 {font-size: 18px;}h6 {font-size: 16px;}ul {margin: 0px;padding: 0px;}li {list-style: none}
	p {
		font-size: 14px;
		font-weight: 500;
		line-height: 26px;
		color: #bcbcbc;
		margin-bottom: 15px;
	}
	hr {
		border-bottom: 1px solid #eceff8;
		border-top: 0 none;
		margin: 30px 0;
		padding: 0;
	}
	img {vertical-align: middle;border-style: none;}
	label {
		color: #7e7e7e;
		cursor: pointer;
		font-size: 14px;
		font-weight: 400;
	}
	*::-moz-selection {
		background: #d6b161;
		color: #fff;
		text-shadow: none;
	}
	::-moz-selection {
		background: #444;
		color: #fff;
		text-shadow: none;
	}
	::selection {
		background: #444;
		color: #fff;
		text-shadow: none;
	}
	*::-moz-placeholder {
		color: #555555;
		font-size: 14px;
		opacity: 1;
	}
	*::placeholder {
		color: #555555;
		font-size: 14px;
		opacity: 1;
	}
	.container, .container-fluid, .container-lg, .container-md, .container-sm, .container-xl {
	    width: 100%;
	    padding-right: 15px;
	    padding-left: 15px;
	    margin-right: auto;
	    margin-left: auto;
	}
	.row {
	    display: -ms-flexbox;
	    display: flex;
	    -ms-flex-wrap: wrap;
	    flex-wrap: wrap;
	    margin-right: -15px;
	    margin-left: -15px;
	}
	.btn:not(:disabled):not(.disabled) {cursor: pointer;}
	.btn {
	    user-select: none;
	    -moz-user-select: none;
	    background: #12151e none repeat scroll 0 0;
	    border: 2px solid #e4d804;
	    border-radius: 50px;
	    color: #e3dfdf;
	    cursor: pointer;
	    display: inline-block;
	    font-size: 12px;
	    font-weight: 700;
	    letter-spacing: 1px;
	    line-height: 1.5;
	    margin-bottom: 0;
	    padding: 16px 34px;
	    text-align: center;
	    text-transform: uppercase;
	    touch-action: manipulation;
	    transition: all 0.3s ease 0s;
	    vertical-align: middle;
	    white-space: nowrap;
	    max-width: 200px;
	}
	.col, .col-1, .col-10, .col-11, .col-12, .col-2, .col-3, .col-4, .col-5, .col-6, .col-7, .col-8, .col-9, .col-auto, .col-lg, .col-lg-1, .col-lg-10, .col-lg-11, .col-lg-12, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8,.col-lg-9, .col-lg-auto, .col-md, .col-md-1, .col-md-10, .col-md-11, .col-md-12, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-auto, .col-sm, .col-sm-1, .col-sm-10, .col-sm-11, .col-sm-12, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-auto, .col-xl, .col-xl-1, .col-xl-10, .col-xl-11, .col-xl-12, .col-xl-2, .col-xl-3, .col-xl-4, .col-xl-5, .col-xl-6, .col-xl-7, .col-xl-8, .col-xl-9, .col-xl-auto {
		position: relative;
		width: 100%;
		padding-right: 15px;
		padding-left: 15px;
	}
</style>
<style name="c_media_query">
	@media (min-width: 576px) {
		.container, .container-sm {max-width: 540px;}
	}
	@media (min-width: 768px) {
		.container, .container-md, .container-sm {max-width: 720px;}
	}
	@media (min-width: 992px) {
		.container, .container-lg, .container-md, .container-sm {max-width: 960px;}
		.col-lg-8 {
		    -ms-flex: 0 0 66.666667%;
		    flex: 0 0 66.666667%;
		    max-width: 66.666667%;
		}
	}
	@media (min-width: 1200px) {
		.container, .container-lg, .container-md, .container-sm, .container-xl {max-width: 1330px;}
	}
</style>
<style name="utilities">
	.mt-25 {margin-top: 25px;}.mb-40 {margin-bottom: 40px;}.f-left {float: left}.f-right {float: right}.fix {overflow: hidden}.uppercase {text-transform: uppercase;}.capitalize {text-transform: capitalize;}.justify-content-center {justify-content: center!important;}.text-center {text-align: center!important;}
</style>
<style name="home_css">
	.tr-movie-bg2 {
	    background-position: top center;
	    background-size: cover;
	    padding: 120px 0 120px;
	}
	.movie-item-row {justify-content: space-between;}
	.tr-movie-btn .btn {
	    letter-spacing: 0;
	    background: #e4d804;
	    color: #1a1e21;
	}
	.tr-movie-btn .btn:hover {
	    background: transparent;
	    color: #fff;
	}
	.title-style-three.text-center {padding-bottom: 30px;}
	.title-style-three {
	    position: relative;
	    padding-bottom: 20px;
	}
	.title-style-three.text-center::before {right: 0;margin: 0 auto;}
	.title-style-three::before {
	    content: "";
	    position: absolute;
	    left: 0;
	    bottom: 0;
	    background-image: url('/web/img/images/title_shape.png');
	    width: 98px;
	    height: 7px;
	}
	.navbar-wrap > ul > li.active > a, .navbar-wrap > ul > li:hover > a, .mobile-menu .navigation li.active > a, .header-lang form .icon, .banner-content .sub-title, .banner-content .title > span, .banner-meta ul li.release-time > span > i, .banner-meta ul li.category > a:hover, .section-title .sub-title, .movie-content .top .date, .movie-content .bottom ul li .quality, .movie-content .bottom ul li > span i, .movie-content .top .title a:hover, .ucm-active .owl-nav button:hover, .ucm-active-two .owl-nav button:hover, .tr-movie-menu-active button.active, .footer-menu nav .navigation li:hover > a, .quick-link-list ul li a:hover, .footer-social ul li a:hover, .copyright-text > p > a, .mobile-menu .social-links li a:hover, .header-top-link .quick-link li a:hover, .header-top-link .header-social li a:hover, .header-top-subs > p > span, .movie-item-two .movie-content .title a:hover, .movie-content-bottom ul li.tag a:hover, .breadcrumb-content .breadcrumb li a, .breadcrumb-content .title > span {
		color: #e4d804;
	}
	.title-style-three .sub-title {font-weight: 700;color: #bcbcbc;}
	.section-title .sub-title {
	    display: block;
	    line-height: 1;
	    font-size: 12px;
	    text-transform: uppercase;
	    font-weight: 900;
	    position: relative;
	    margin-bottom: 12px;
	    letter-spacing: 1px;
	}
	.section-title .title {margin-bottom: 0;font-size: 36px;}
	.movie-item-row .custom-col- {
	    -ms-flex: 0 0 19.2%;
	    flex: 0 0 19.2%;
	    max-width: 19.2%;
	    width: 100%;
	    padding-right: 15px;
	    padding-left: 15px;
	}
	.movie-item-row .custom-col- .movie-item-two {margin-bottom: 45px;}
	.movie-item-two {
	    text-align: center;
	    background: #1f1e24;
	    padding: 15px 15px 25px;
	}
	.movie-poster {margin-bottom: 23px;position: relative;}
	.movie-item-row .movie-poster {position: relative;}
	.movie-content {padding-right: 10px;}
	.movie-item-two .movie-content {padding: 0;}
	.movie-item-row .movie-poster::before, .movie-item-three .movie-poster::before {
	    content: "";
	    position: absolute;
	    left: 0;
	    top: 0;
	    width: 100%;
	    height: 100%;
	    background: #04050a;
	    transition: .3s linear;
	    opacity: 0;
	}
	.movie-poster img {max-width: 100%;border-radius: 5px;}
	.movie-item-two .movie-content > .rating {
	    font-size: 10px;
	    letter-spacing: -.5px;
	    color: #e4d804;
	    margin-bottom: 10px;
	}
	.movie-item-two .movie-content > .rating svg {width: 17px;}
	.movie-item-two .movie-content .title {
	    font-size: 16px;
	    font-weight: 600;
	    color: #d5d5d5;
	    margin-bottom: 12px;
	}
	.movie-item-two .movie-content .rel {
	    display: block;
	    font-size: 12px;
	    color: #9d9b9b;
	    font-weight: 900;
	    letter-spacing: 0.6px;
	}
	.movie-content-bottom ul {
	    display: flex;
	    align-items: center;
	    justify-content: space-between;
	    padding-top: 15px;
	    margin-top: 25px;
	    position: relative;
	}
	.movie-content-bottom ul::before {
	    content: "";
	    position: absolute;
	    left: 0;
	    top: 0;
	    width: 100%;
	    height: 1px;
	    background: #000000;
	}
	.movie-content-bottom ul::after {
	    content: "";
	    position: absolute;
	    left: 0;
	    top: 1px;
	    width: 100%;
	    height: 1px;
	    background: #27272f;
	}
	.movie-content-bottom ul li.tag {
	    display: flex;
	    flex-wrap: wrap;
	    flex-grow: 1;
	    margin-right: 30px;
	}
	.movie-content-bottom ul li.tag a {
	    display: block;
	    color: #a2a2a5;
	    background: #02050a;
	    font-size: 12px;
	    font-weight: 700;
	    padding: 7px 12px;
	    line-height: 1;
	    margin-right: 10px;
	}
	.movie-content-bottom ul li .like {font-size: 13px;color: #9d9b9b;}
	.movie-content-bottom ul li .like .svg-inline--fa.fa-thumbs-up.fa-w-16 {
	    width: 12px;
	    margin-right: 5px;
	    color: #c77f01;
	}
	.tr-movie-menu-active {
	    display: flex;
	    align-items: center;
	    flex-wrap: wrap;
	    justify-content: center;
	    margin-bottom: 40px;
	}
	.tr-movie-menu-active button {
	    border: none;
	    border-radius: 4px;
	    box-shadow: inset 0px 3px 7px 0px rgb(0 0 0 / 77%);
	    background: #0b1110;
	    font-size: 13px;
	    text-transform: uppercase;
	    font-weight: 900;
	    color: #cdcaca;
	    padding: 17px 25px;
	    position: relative;
	    margin: 0 7.5px 15px;
	}
	.tr-movie-menu-active button.active::before, .tr-movie-menu-active button.active::after {opacity: 1;}
	.tr-movie-menu-active button.active {text-shadow: 0px 3px 24px rgb(228 216 4 / 50%);}
	.tr-movie-menu-active button::before, .tr-movie-menu-active button::after {
	    content: "";
	    position: absolute;
	    left: 0;
	    top: 50%;
	    transform: translateY(-50%);
	    width: 2px;
	    height: 16px;
	    transition: .3s linear;
	    opacity: 0;
	}
	.tr-movie-menu-active button::after {left: auto;right: 0;}
	.scroll-top, .btn:hover, .navbar-wrap > ul > li .submenu li a::before, .title-style-two .sub-title::before, .services-list ul li .icon::before, .tr-movie-menu-active button::before, .tr-movie-menu-active button::after {background: #e4d804;}
	[type=button]:not(:disabled), [type=reset]:not(:disabled), [type=submit]:not(:disabled), button:not(:disabled) {cursor: pointer;}
</style>