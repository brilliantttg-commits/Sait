@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&family=Saira+Stencil+One&display=swap');
@import url('./base.css');

:root {
  --viollet: #3e284f;
  --LightViollet: #775194;
  --white: #fff;
  --green: #00a441;
  --black: #404040;
  --grey: #eee;
  --lightGrey: #f4f4f4;
  --darkGrey: #bbb;
  --font: 'Saira Stencil One', sans-serif;
  --fontOpen: 'Open Sans', sans-serif;
}

.wrapper__nav {
  background: var(--viollet);
  box-shadow: 0px 0px 20px 0px #3e284f80;
}

.wrapper__navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 15px;
}

.logo {
  display: flex;
  align-items: center;
  gap: 12px;
  color: var(--white);
  font-family: var(--font);
  font-size: 18px;
  font-weight: 400;
}

.wrapper__navbar-right {
  position: relative;
}

.wrapper__navbar-btn {
  position: relative;
  z-index: 10;
}

.wrapper__navbar-btn-counter {
  position: absolute;
  width: 18px;
  height: 18px;
  background: var(--white);
  border-radius: 50%;
  border: 1px solid var(--viollet);
  top: -9px;
  right: -9px;
  font-family: var(--fontOpen);
  font-size: 12px;
  font-weight: 300;
  display: flex;
  justify-content: center;
  align-items: center;
  transform: scale(0);
  transition: 0.5s;
}
.wrapper__navbar-btn-counter.active {
  transform: scale(1);
}

.wrapper__navbar-basket {
  position: absolute;
  top: 65px;
  right: 0;
  background: var(--white);
  box-shadow: 0px 4px 10px 0px #0000001a;
  width: 358px;
  height: 392px;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  border-radius: 10px;
  transition: 0.5s;
  transform: translateY(-150%);
  opacity: 0;
}

.wrapper__navbar-basket.active {
  transform: translateY(0%);
  opacity: 1;
}

.wrapper__navbar-basket-top {
  background: var(--LightViollet);
  padding: 13px 16px;
  border-radius: 10px 10px 0 0;
  font-family: var(--fontOpen);
  font-size: 16px;
  font-weight: 700;
  color: var(--white);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.wrapper__navbar-basket-bottom {
  background: var(--green);
  padding: 13px 16px;
  border-radius: 0 0 10px 10px;
  font-family: var(--fontOpen);
  font-size: 16px;
  font-weight: 700;
  color: var(--white);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.wrapper__navbar-basket-checklist {
  height: 100%;
  padding: 16px;
  background: var(--white);
}

.wrapper__navbar-product {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 15px;
}

.wrapper__navbar-info {
  display: flex;
  align-items: center;
  gap: 10px;
}

.wrapper__navbar-productImage {
  width: 70px;
  height: 54px;
}

.wrapper__navbar-infoName {
  font-family: var(--font);
  font-size: 16px;
  font-weight: 400;
}
.wrapper__navbar-infoPrice {
  font-family: var(--fontOpen);
  font-size: 16px;
  font-weight: 400;
}

.wrapper__navbar-option {
  display: flex;
  justify-content: center;
  align-items: center;
  background: var(--darkGrey);
  border-radius: 4px;
  overflow: hidden;
  border: 1px solid var(--darkGrey);
}

.wrapper__navbar-symbol {
  width: 25px;
  height: 25px;
  font-family: var(--fontOpen);
  font-size: 16px;
  font-weight: 700;
  transition: 0.3s;
}

.wrapper__navbar-count {
  width: 40px;
  height: 25px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  background: var(--grey);
}

.fa-minus:hover {
  background: red;
  color: var(--white);
}
.fa-plus:hover {
  background: var(--green);
  color: var(--white);
}

.wrapper__view {
  position: relative;
  z-index: -2;
  margin-top: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.wrapper__view img {
  width: 85%;
  display: block;
}

.wrapper__list {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 75px;
  gap: 24px;
}

.wrapper__list-card {
  position: relative;
  text-align: center;
  border-radius: 10px;
  box-shadow: 0px 20px 20px -15px #00000040;
  background: var(--lightGrey);
  padding: 16px;
  width: 306px;
}

.wrapper__list-card-img {
  margin-top: -75px;
}

.wrapper__list-card-sub {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
}

.wrapper__list-card-title {
  font-family: var(--font);
  font-size: 18px;
  font-weight: 400;
  margin-top: 10px;
}
.wrapper__list-price {
  font-family: var(--fontOpen);
  font-size: 16px;
  font-weight: 700;
  padding: 10px;
  border-radius: 10px;
  background: var(--viollet);
  color: var(--white);
}

.wrapper__list-btn {
  padding: 10px;
  border-radius: 10px;
  background: var(--viollet);
  color: var(--white);
  display: flex;
  justify-content: center;
  align-items: center;
  transition: 0.3s;
}
.wrapper__list-btn:hover {
  background: var(--green);
}

.wrapper__list-card-count {
  position: absolute;
  width: 30px;
  height: 30px;
  top: -15px;
  right: -15px;
  border: 2px solid var(--white);
  background: var(--viollet);
  border-radius: 50%;
  color: var(--white);
  font-family: var(--fontOpen);
  font-size: 12px;
  font-weight: 400;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: 0.5s;
  opacity: 0;
}
.wrapper__list-card-count.active {
  opacity: 1;
}

.print {
  width: 200px;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 5px;
  background: #fff;
  border-radius: 10px;
  height: 300px;
}

.print__header {
  display: flex;
  align-items: center;
  gap: 10px;
}
.print__header img {
  filter: invert();
}
.print__body {
  display: flex;
  flex-direction: column;
  width: 100%;
  gap: 10px;
  margin: 20px 0;
}
.print__body-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
}
.print__body-name {
  display: flex;
  align-items: center;
  gap: 10px;
}
.print__footer {
  display: flex;
  justify-content: center;
  align-items: center;
}
.modal {
  position: fixed;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  background: #000000de;
  align-items: center;
  justify-content: center;
  display: none;
}
.modal.active {
  display: flex;
}
