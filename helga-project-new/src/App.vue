<script setup>
import { ref } from 'vue'
const menuIsOpen = ref(false)

const toggleMenu = () => {
menuIsOpen.value = !menuIsOpen.value
}
</script>

<template>

	<header class="header">
		<div class="header__content container">
			<div class="burger"  :class="{ 'active': menuIsOpen }" @click="menuIsOpen = !menuIsOpen">
				<span></span><span></span><span></span>
			</div>
				<div class="mobile-menu container" :class="{ 'active': menuIsOpen }" @click="menuIsOpen = !menuIsOpen">
				<div class="mobile-menu__header">
					<h4>Меню</h4>
				<div class="burger" :class="{ 'active': menuIsOpen }">
					<span></span>
					<span></span>
					<span></span>
				</div>
			</div>
			<div class="mobile-menu__body">
				<nav class="mobile-menu__menu">
					<a href="#" class="mobile-menu__nav-item">Каталог</a>
					<a href="#" class="mobile-menu__nav-item">Советы по уходу</a>
					<a href="#" class="mobile-menu__nav-item">Оплата и доставка</a>
					<a href="#" class="mobile-menu__nav-item">Контакты</a>
				</nav>
			</div>
		</div>
			<div class="header__logotip">
				<a href="#" class="header__logotip-link"><h2 class="header__logo"> Plant </h2></a>
			</div>
			<nav class="header__menu">
				<a href="#" class="header__nav-item">Каталог</a>
				<a href="#" class="header__nav-item">Советы по уходу</a>
				<a href="#" class="header__nav-item">Оплата и доставка</a>
				<a href="#" class="header__nav-item">Контакты</a>
			</nav>
				<div class="header__icons">
					<a href="#" class="header__icon-link"><img class="header__icon" src="./assets/images/loupe.svg" alt=""></a>
					<a href="#" class="header__icon-link"><img class="header__icon" src="./assets/images/enter.svg" alt=""></a>
					<a href="#" class="header__icon-link"><img class="header__icon" src="./assets/images/basket.svg" alt=""></a>
				</div>
		</div>
	</header>

	<div class="main">
		<div class="main__content container">
			<div class="main__img">
				<div class="main__describe">
					<h1 class="main__head">
						Цветы для вашего дома
					</h1>
						<div class="main__text">
							Растения в кашпо станут красивым и модным дополнением вашей квартиры или офиса
						</div>
					<button type="button" class="main__button">
						ПЕРЕЙТИ В КАТАЛОГ
					</button>
				</div>
			</div>
			<div class="main__items">
				<div class="main__item">
					<a href="#" class="main__item-img"><img src="./assets/images/product-ficus.jpg" alt="" class="main__product"></a>
						<h2 class="main__title">
							<a href="#" class="main__title-link">Фикусы</a>
						</h2>
							<div class="main__subtitle">
								Эффектные украшения интерьера
							</div>
				</div>
				<div class="main__item">
					<a href="#" class="main__item-img"><img src="./assets/images/product-sycculent.jpg" alt="" class="main__product"></a>
						<h2 class="main__title">
							<a href="#" class="main__title-link">Суккуленты</a>
						</h2>
							<div class="main__subtitle">
								Маленькие и модные
							</div>
						</div>
				<div class="main__item main__item--palm">
					<a href="#" class="main__item-img"><img src="./assets/images/product-palm.jpg" alt="" class="main__product main__product--palm"></a>
						<h2 class="main__title">
							<a href="#" class="main__title-link">Пальмы</a>
						</h2>
							<div class="main__subtitle">
								Пышные и неприхотливые пальмы - элегантный пример декора
							</div>
					</div>
				</div>	
			</div>
		</div>

	<div class="offer">
			<div class="offer__content container"> 
				<h3 class="offer__head">
					Предложение месяца
				</h3>
				<div class="offer__first-row">
					<div class="offer__product">
						<a href="#" class="offer__product-img"> <img src="./assets/images/product-alokazia.png" alt="" class="offer__product-image"></a>
						<div class="offer__subtitle">
							<a href="#" class="offer__subtitle-link">Ароидные</a>
						</div>
						<div class="offer__title">
							<a href="#" class="offer__title-link">АЛОКАЗИЯ ВЕНТИ</a>
						</div>
						<div class="offer__price">
							1790 ₽
						</div>
					</div>

					<div class="offer__product">
						<a href="#" class="offer__product-img"> <img src="./assets/images/product-bonsay.png" alt="" class="offer__product-image"></a>
						<div class="offer__subtitle">
							<a href="#" class="offer__subtitle-link">Самшиты</a>
						</div>
						<div class="offer__title">
							<a href="#" class="offer__title-link">БОНСАЙ</a>
						</div>
						<div class="offer__price">
							2390 ₽
						</div>
					</div>

					<div class="offer__product">
						<div class="offer__sale">-32%</div>
						<a href="#" class="offer__product-img"> <img src="./assets/images/product-strelicia-nikolaya.png" alt="" class="offer__product-image"></a>
						<div class="offer__subtitle">
							<a href="#" class="offer__subtitle-link">Фикусы</a>
						</div>
						<div class="offer__title">
							<a href="#" class="offer__title-link">СТРЕЛИЦИЯ НИКОЛАЯ</a>
						</div>
						<div class="offer__price offer__price_sale">
							<div class="offer__old-price">
								1890 ₽
							</div>
							<div class="offer__new-price">
								1290 ₽
							</div>
						</div>
					</div>

					<div class="offer__product">
						<a href="#" class="offer__product-img"> <img src="./assets/images/product-fikus-lirovidnui.png" alt="" class="offer__product-image"></a>
						<div class="offer__subtitle">
							<a href="#" class="offer__subtitle-link">Фикусы</a>
						</div>
						<div class="offer__title">
							<a href="#" class="offer__title-link">ФИКУС ЛИРОВИДНЫЙ</a>
						</div>
						<div class="offer__price">
							1490 ₽
						</div>
					</div>
				</div>

				<div class="offer__second-row">
					<div class="offer__product">
						<a href="#" class="offer__product-img"> <img src="./assets/images/product-fikus-elastika.png" alt="" class="offer__product-image"></a>
						<div class="offer__subtitle">
							<a href="#" class="offer__subtitle-link">Фикусы</a>
						</div>
						<div class="offer__title">
							<a href="#" class="offer__title-link">ФИКУС ЭЛАСТИКА</a>
						</div>
						<div class="offer__price">
							3590 ₽
						</div>
					</div>

				
					<div class="offer__product">
						<div class="offer__sale">-50%</div>
						<a href="#" class="offer__product-img"> <img src="./assets/images/product-zamiokulkas.png" alt="" class="offer__product-image"></a>
						<div class="offer__subtitle">
							<a href="#" class="offer__subtitle-link">Ароидные</a>
						</div>
						<div class="offer__title">
							<a href="#" class="offer__title-link">ЗАМИОКУЛЬКАС</a>
						</div>
						<div class="offer__price offer__price_sale">
							<div class="offer__old-price">
								2780 ₽
							</div>
							<div class="offer__new-price">
								1390 ₽
							</div>
						</div>
					</div>

					<div class="offer__product">
						<a href="#" class="offer__product-img"> <img src="./assets/images/pruduct-sanseveria.png" alt="" class="offer__product-image"></a>
						<div class="offer__subtitle">
						<a href="#" class="offer__subtitle-link">Спаржевые</a>
						</div>
						<div class="offer__title">
							<a href="#" class="offer__title-link">САНСЕВИЕРИЯ</a>
						</div>
						<div class="offer__price">
							3790 ₽
						</div>
					</div>

					<div class="offer__product">
						<div class="offer__sale">-25%</div>
						<a href="#" class="offer__product-img"> <img src="./assets/images/product-kaktus.png" alt="" class="offer__product-image"></a>
						<div class="offer__subtitle">
							<a href="#" class="offer__subtitle-link">Кактусовые</a>
						</div>
						<div class="offer__title">
							<a href="#" class="offer__title-link">КАКТУС</a>
						</div>
						<div class="offer__price offer__price_sale">
							<div class="offer__old-price">
								1290 ₽
							</div>
							<div class="offer__new-price">
								970 ₽
							</div>
						</div>
					</div>
				</div>
					<button type="button" class="offer__button">
						ПЕРЕЙТИ В КАТАЛОГ
					</button>
		</div>
	</div>

	<footer class="footer">
		<div class="footer__content container">
			<div class="footer__content-left">
				<nav class="footer__nav">
					<a class="footer__nav-item" href="#">Каталог</a>
					<a class="footer__nav-item" href="#">Советы по уходу</a>
					<a class="footer__nav-item" href="#">Оплата и доставка</a>
					<a class="footer__nav-item" href="#">Контакты</a>
				</nav>
					<div class="footer__logotip">
						<a href="#"><h2 class="footer__logo"> Plant </h2></a>
						<div class="footer__describe">
							© 2023 магазин цветов и растений PLANT
						</div>
					</div>
				</div>
					<div class="footer__content-right">
						<div class="footer__icons">
							<a href="#" class="footer__icons-link"><img class="footer__icon" src="./assets/images/icon-telegram.png" alt=""></a>
							<a href="#" class="footer__icons-link"><img class="footer__icon" src="./assets/images/icon-vk.png" alt=""></a>
							<a href="#" class="footer__icons-link"><img class="footer__icon" src="./assets/images/icon-f.png" alt=""></a>
						</div>
					<form action="post" class="footer__form">
						<input type="text" name="e_mail" placeholder="E-mail" class="footer__input-text">
						<input type="submit" value="ПОДПИСАТЬСЯ" class="footer__input-button">
					</form>
				</div>
		</div>
	</footer>	
	
</template>


<style
	lang="scss">

body {
	margin: 0;
	padding: 0;
}

.container {
	max-width: 1250px;
	margin: 0 auto;
	padding: 0 20px;
	box-sizing: border-box;
}

a:active {
	color: #363434;
	font-weight: 600;
}

a:hover {
	color: #363434;
}
		
.header {
	margin-bottom:30px;

	&__content {
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	&__logo {
		color: #1F650D;
		font-family: Marko One;
		font-size: 40px;	
	}
		
	&__menu {
		display: flex;
		align-items: center;
		gap: 53px;	
	}

	&__nav-item {
		color: #898080;
		font-family: Open_Sans;
		font-size: 14px;
		font-style: normal;
		text-decoration: none;
	}

	&__icons {
		display: flex;
		align-items: flex-start;
		gap: 24px;
	}

	&__logotip a{
			text-decoration: none;
	} 
}

.main {
	margin-bottom: 97px;

	&__img {
		background: url(./assets/images/banner.jpg);
		background-repeat: no-repeat;
   		background-position: center;
    	background-size: cover;
		margin-bottom: 80px;
		padding-bottom: 20px;
	}
		
	&__describe {
		display: flex;
		flex-direction: column;
		padding-left: 100px;
	}
	
	&__banner {
		width: 100%;
		margin: 0 auto;
	}
		
	&__head {
		max-width: 300px;
		color: #262323;
		font-family: Open_Sans;
		font-size: 44px;
	}

	&__text {
		max-width: 405px;
		color: #565252;
		font-family: Open_Sans;
		font-size: 18px;
		font-weight: 400;
		margin-bottom: 59px;
	}
	
	&__button {
		font-family: Open_Sans;
		width: 170px;
		height: 55px;
		background-color: #6D6666;
		color: #ffffff;
		font-size: 12px;
		border: none;
	}
		&__button:hover {
			background-color: #FCF5F5;
			color: #535050;
			box-shadow: 1px 0px 4px 0px rgba(0, 0, 0, 0.25), 1px 2px 4px 0px rgba(0, 0, 0, 0.25);
		}

	&__items {
		display: flex;
		justify-content: space-between;
	}

	&__product{
		width: 100%;
	}
	
	&__title {
		margin: 7px 0;	
	}

	&__title-link {
		font-family: Open_Sans;
		font-size: 18px;
		color: #010101;
		text-decoration: none;
	}
	
	&__subtitle {
		color: rgba(1, 1, 1, 0.73);
		font-family:Open_Sans;
		font-size: 14px;
	}

}

.offer {

	.offer__content {
		margin-bottom: 170px;
	}
	
	&__head {
		font-family: Open_Sans;
		font-size: 26px;
		color: #000;
		margin-bottom: 40px;
	}

	&__first-row {
		display: flex;
		justify-content: space-between;
		margin-bottom: 45px;
	}

	&__second-row {
		display: flex;
		justify-content: space-between;
		margin-bottom: 118px;
	}
			
	&__product {
		display: inline-block;
		position: relative;
	}

	&__product-image {
		width: 100%;
	}
	
	&__sale {
		width: 61px;
		height: 22px;
		background: rgba(245, 81, 81, 0.97);
		font-family:Martel_Sans-bold;
		font-size: 14px;
		color: #FFF;
		position: absolute;
		top: 26px;
		text-align: center;
	}

	&__subtitle {
		margin: 7px 0;	
	}
		
	&__title {
		margin-bottom: 5px;
	}
		
	&__subtitle-link {
		font-family: Open_Sans;
		font-size: 12px;
		color: #7C7C7C;
		text-decoration: none;
	}
		
	&__title-link {
		font-family: Open_Sans;
		font-size: 14px;
		color: #010101;
		text-decoration: none;
	}

	&__price {
		font-family: Martel_Sans-bold;
		font-size: 16px;
		color: #211F1F;
		text-align: right;
	}

	&__old-price {
		display: inline-block;
		font-family: Martel_Sans-light;
		font-size: 16px;
		color:  #B2B1B1;
		text-decoration: line-through;
		text-decoration-color: #B2B1B1;
	}

	&__new-price {
		display: inline-block;
		font-family: Martel_Sans-bold;
		font-size: 16px;
		color: #F55;
	}
	
	&__price_sale {
		display: flex;
		justify-content: space-between;

	}

	&__button {
		width: 280px;
		height: 54px;
		background-color: #759E67;
		border: none;
		color: #F6F6F6;
		font-family: Open_Sans;
		font-size: 16px;
		margin-left: auto;
		margin-right: auto;
		display: block;
		
	}
		&__button:hover {
			background-color: #52A635;
			box-shadow: 1px 0px 4px 0px rgba(0, 0, 0, 0.25), 1px 2px 4px 0px rgba(0, 0, 0, 0.25);
		}
}

.footer {
	background-color: rgba(85, 85, 85, 0.99);

	&__content {
		display: flex;
		justify-content: space-between;
	}
	
	&__nav {
		display:flex;
		gap: 45px;
		margin-top: 35px;
		margin-bottom: 35px;
	}
	
	&__nav-item {
		font-family: Open_Sans;
		color: #DEDEDE;
		font-size: 12px;
		text-decoration: none;
	}

	&__logotip {
		margin-bottom: 15px;
	}

	&__logotip a {
		margin-bottom: 15px;
		text-decoration: none;
	}

	&__logo {
		font-family: Marko One;
		color: #FBFBFB;
		font-size: 22px;
		margin-bottom: 10px;
	}

	&__describe {
		font-family: Open_Sans;
		color: #DEDEDE;
		font-size: 12px;
	}
	
	&__icons {
		display: flex;
		justify-content: end;
		gap: 15px;
		margin-top: 35px;
		margin-bottom: 45px;
	}

	&__form {
		display: flex;
		gap: 10px;
		margin-bottom: 15px;
	}

	&__input-text {
		color: rgba(251, 251, 251, 0.37);
		font-family: Open_Sans;
		font-size: 14px;
		width: 178px;
		height: 27px;
		border: 1px solid #FBFBFB;
		background: #575757;
		outline: none;
	}

	&__input-button {
		color: #000;
		font-family: Open_Sans;
		font-size: 12px;
		width: 135px;
		height: 31.3px;
		background: rgba(251, 251, 251, 0.91);
		border: none;
	}

	&__input-button:active {
		background: #363434;
		color: #FBFBFB;
	}	
}

.burger {
	display: none;
	position: relative;
	width: 40px;
	height: 40px;
	border: none;
	background-color: transparent;

	& span {
	position: absolute;
	width: 30px;
	height: 2px;
	background-color: #000;
	left: 5px;
	transition: transform .5s, opacity .5s, background-color .5s;
	}
	&.active {
	border: 1.6px solid hsla(0,0%,100%,.2);
    border-radius: 999px;
	}
	&.active span {
	background-color: hsla(0,0%,100%,.2);
	top: 18px;
	}
	&.active span:nth-child(1) {
		opacity: 0;
	}
	&.active span:nth-child(2) {
		transform: translateY(0) rotate(45deg);
	}
	&.active span:nth-child(3) {
		transform: translateY(0) rotate(-45deg);
	}
	& span:nth-child(1) {
	transform: translateY(20px);
	}
	& span:nth-child(2) {
	transform: translateY(10px);
	}
	& span:nth-child(3) {
	transform: translateY(30px);
	}
}

.mobile-menu {
	position: fixed;
    top: 0;
    left: -120%;
    width: 100%;
    height: 100%;
    background: #5dc067;
    padding: 20px;
    display: flex;
    flex-direction: column;
    overflow: auto;
    transition: all .3s ease;

	&__header {
	display: flex;
    align-items: center;
    justify-content: space-between;
	}
	&__header h4 {
	font-family: Open_Sanspen;
	font-weight: 400;
    font-size: 18px;
    color: hsla(0,0%,100%,.2);
	}
	&__body {
	margin: auto 0;
    padding: 60px 0;
	}
	&.active {
	left: 0;
	}	
	&__menu {
		display: flex;
		flex-direction: column;
		margin: 0;
	}
	&__nav-item {
		font-family: Open_Sans;
		font-size: 24px;
		color: #ffffff;
		line-height: 45px;
		margin: 0;
		padding: 16px 0;
		border-bottom: 1px solid hsla(0,0%,100%,.2);
		width: 100%;
		text-decoration: none;
	}
	&__nav-item:first-child {
		border-top: 1px solid hsla(0,0%,100%,.2);
	}
}


@media (max-width: 1200px) {
	.main__head {
		max-width: 600px;
		font-size: 36px;
		margin-bottom: 40px;
	}
	.main__text {
		max-width: 405px;
		font-size: 16px;
		margin-bottom: 59px;
	}
	.main__button {
		width: 150px;
		height: 45px;
		font-size: 11px;
		border: none;
	}
	.main__items {
		gap: 35px;
	}
	.offer__product {
		border: 1px solid #eeeeeedb;
	}
	.offer__first-row {
		gap: 35px;
	}
	.offer__second-row {
		gap: 35px;
	}
}


@media (max-width: 960px) {
	.burger {
	display: flex;
	}
	.header__logo {
		color: #1F650D;
		font-family: Marko One;
		font-size: 34px;
	}
	.header__nav {
		gap: 20px;
	}
	.header__menu {
		display: none;
	}
	.main__describe {
		top: 10px;
		left: 80px;
	}
	.main__head {
		max-width: 600px;
		font-size: 30px;
		margin-bottom: 25px;
	}
	.main__text {
		max-width: 350px;
		font-size: 12px;
		margin-bottom: 49px;
	}
	.main__button {
		width: 140px;
		height: 40px;
		font-size: 11px;
		border: none;
	}
}


@media (max-width: 768px) {

	.header {
		margin-bottom:10px;
	}

	.footer__nav-item {
		font-family: Open_Sans;
		color: #DEDEDE;
		font-size: 11px;
		text-decoration: none;
	}
	.main__banner {
		height: 200px;
	}
	.main__head {
		max-width: 600px;
		font-size: 24px;
		margin-bottom: 25px;
	}
	.main__text {
		max-width: 300px;
		font-size: 11px;
		margin-bottom: 29px;
	}
	.main__describe {
		padding-top: 10px;
		padding-left: 60px;
	}
	.main__button {
		width: 120px;
		height: 33px;
		font-size: 8px;
		border: none;
	}
	.main__item--palm {
		width: 100%;
	}
	.main__items {
		flex-wrap: wrap;
	}
	.main__item:not(:last-child) {
            flex-basis: 44%;
        }
	.header__icons {
		gap: 20px;
	}
}


@media (max-width: 689px) {
	.main {
		margin-bottom: 50px;
	}
	.main__head {
		font-size: 16px;
		margin-bottom: 15px;
	}
	.main__text {
		max-width: 250px;
		font-size: 10px;
		margin-bottom: 20px;
		line-height: 120%;
		
	}
	.main__describe {
		padding-left: 30px;
	}
	.main__button {
		width: 80px;
		height: 20px;
		font-size: 6px;
	}
	.main__item {
		border: 1px solid #eeeeeedb;
		font-size: 10px;
	}
	.main__items {
		flex-wrap: wrap;
	}

	.main__title {
		margin: 4px 0;	
	}
	.main__title-link {
		font-family: Open_Sans;
		font-size: 16px;
	}
	.main__subtitle {
		font-size: 12px;
	}
	.main__img {
		margin-bottom: 50px;
	}
	.main__banner {
		height: 130px;
	}
	.offer__head {
		font-size: 22px;
		margin-bottom: 30px;
	}
	.offer__first-row {
		flex-wrap: wrap;
	}
	.offer__second-row {
		flex-wrap: wrap;
	}
	.offer__product {
		flex-basis: 44%;
	}
	.offer__button {
		width: 200px;
   		height: 44px;
		font-size: 14px;
	}

	.footer__content {
		display: flex;
		flex-direction: column;
	}
	
	.footer__nav {
		gap: 25px;
		margin-top: 35px;
		margin-bottom: 15px;
		flex-direction: column;
		justify-content: space-between;
	}
	
	.footer__nav-item {
		font-family: Open_Sans;
		color: #DEDEDE;
		font-size: 16px;
		text-decoration: none;
	}

	.footer__logotip {
		display: none;
	}

	.footer__logotip a {
		margin-bottom: 15px;
		text-decoration: none;
	}

	.footer__logo {
		font-family: Marko One;
		color: #FBFBFB;
		font-size: 22px;
		margin-bottom: 10px;
	}

	.footer__describe {
		font-family: Open_Sans;
		color: #DEDEDE;
		font-size: 12px;
	}
	
	.footer__icons {
		display: inline-flex;
		justify-content: start;
		gap: 25px;
	}

	.footer__icon {
		width: 130%;
	}

	.footer__form {
		display: inline-flex;
	}

	.footer__input-text {
		display: none;
	}

	.footer__input-button {
		background-color: #363434;
		color: #DEDEDE;
		font-size: 10px;
		width: 130px;
	}
	.footer__content-right {
		display: inline-flex;
		justify-content: space-between;
		align-items: center;
	}
}			


</style>
