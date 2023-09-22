
import { setBlockTracking } from 'nuxt/dist/app/compat/capi';
<template>
  <header class="text-center">
      <p class="mt-14 mb-6 text-lg text-gray-300">Вища Бухгалтерська Online-Академія</p>
      <h1 class="text-4xl mb-6 font-bold tracking-tight">Підвищення кваліфікації
    <br> та профперепідготовка для бухгалтерів</h1>
      <button class="mb-10 px-6 py-3 bg-blue-600 text-white font-semibold rounded-full hover:bg-indigo-700 focus:outline-none focus:ring-indigo-700">
          Обрати навчання >>
      </button>

      <div class="flex justify-center items-center">
          <img class="" src="~/assets/images/photo1.png" alt="photo1">
          <img class="" src="~/assets/images/photo2.png" alt="photo2">
          <img class="" src="~/assets/images/photo3.png" alt="photo3">
      </div>

      <h3 class="text-3xl mt-10">Разом дешевше! Купуйте передплату на Вищу Бухгалтерську <br> 
    Online-Академію <span class="text-blue-600">8 професій за ціною 2</span></h3>

      <div class="mt-8 mb-16 bg-gray-100 text-white text-center py-6">
          <h1 class="text-2xl text-gray-100">.</h1>
      </div>

      <h1 class="mb-10 text-4xl">Навчання, яке працює!<br>
    Відкрийте для себе найпопулярніші курси
  </h1>

      <div class="timeline-title">
          <ul class="flex justify-between mx-64 text-gray-500">
              <li class="px-4"><span>Ціни раннього бронювання</span></li>
              <li class="px-4"><span>Подорожання на 10%</span></li>
              <li class="px-4"><span>Подорожання на 15%</span></li>
              <li class="px-4"><span>Квитки вже закінчаться</span></li>
          </ul>
      </div>

      <div class="mb-10 flex justify-center items-center relative">
          <div class="timeline-container">
              <ul class="base-timeline">
                <li class="base-timeline__item ml-0 pr-10">
                  <span class="base-timeline__summary-text text-white">21</span>
                </li>
                <li class="base-timeline__item ml-10">
                  <span class="base-timeline__summary-text">21 серпня</span>
                </li>
                <li class="base-timeline__item ml-20">
                  <span class="base-timeline__summary-text">1 вересня</span>
                </li>
                <li class="base-timeline__item ml-40">
                  <span class="base-timeline__summary-text">15 вересня</span>
                </li>
                <li class="base-timeline__item ml-60">
                  <span class="base-timeline__summary-text">3 жовтня</span>
                </li>
              </ul>
              <div class="timeline-circle" ref="timelineCircle"></div>
          </div>
      </div>

  </header>

  <div class="bg-gray-100">
      <section class="mx-64 text-center">
          <h1 class="mt-28 text-4xl">Передплата на Вищу Бухгалтерську<br>
    Онлайн-Академію
  </h1>
          <p class="mt-4 mb-6 text-lg">Оберіть свій тарифний пакет:</p>

          <div class="flex justify-between">
              <div>
                  <div class="mt-16 text-blue-500 py-2 px-4 rounded-lg inline-flex items-center space-x-2">
                      <span class="text-lg font-semibold">
                        {{ countdown.hours + `  :` }} <br>год.
                    </span>
                      <span class="text-lg font-semibold">
                        {{ countdown.minutes + `  :` }} <br>хв.
                    </span>
                      <span class="text-lg font-semibold">
                        {{ countdown.seconds }} <br>сек.
                      </span>
                  </div>
                  <p>(для діючих передплатників
                      <br> додаткова знижка 10%)</p>
              </div>

              <div class="flex">
                  <div class="">
                      <div class="mb-4">
                          <p class="mb-4 mr-4 inline-block">СУПЕРПРОФЕСІОНАЛ</p>
                          <button class="px-1 py-3 bg-blue-600 text-white font-semibold rounded-full hover:bg-indigo-700 focus:outline-none focus:ring-indigo-700 inline-block">-75%</button>
                      </div>
                      <p class="mb-4">8 професійних курсів
                          <br> за ціною 2</p>
                      <p class="mb-2">1070 грн/міс</p>
                      <p class="mb-4">679 грн/міс</p>
                      <button class="mb-2 px-10 py-3 bg-blue-600 text-white font-semibold rounded-full hover:bg-indigo-700 focus:outline-none focus:ring-indigo-700">
                          Оплатити карткою
                      </button>
                      <p class="mb-2">Оплатити частинами</p>
                  </div>
                  <div class="ml-10">
                      <div class="mb-4">
                          <p class="mb-4 mr-4 inline-block">СУПЕРПРОФЕСІОНАЛ</p>
                          <button class="px-1 py-3 bg-blue-600 text-white font-semibold rounded-full hover:bg-indigo-700 focus:outline-none focus:ring-indigo-700 inline-block">-75%</button>
                      </div>
                      <p class="mb-4">8 професійних курсів
                          <br> за ціною 2</p>
                      <p class="mb-2">1070 грн/міс</p>
                      <p class="mb-4">679 грн/міс</p>
                      <button class="mb-2 px-10 py-3 bg-blue-600 text-white font-semibold rounded-full hover:bg-indigo-700 focus:outline-none focus:ring-indigo-700">
                          Оплатити карткою
                      </button>
                      <p class="mb-2">Оплатити частинами</p>
                  </div>
              </div>
          </div>
          <div class="">
              <ul class="mb-10">
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Поглиблені професійні курси підвищення <br> кваліфікації (8 курсів/рік)</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Поглиблені професійні курси підвищення <br> кваліфікації (8 курсів/рік)</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Практичні курси автоматизації <br>(робота в BAS, Medoc, Excel, ЕК)</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Закриті клубні лекції з експертами (1 <br>р./ міс.)</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Майстер-класи зі змін у законодавстві  (4+ <br>р./міс.)</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Безлімітні відповіді на запитання під час <br>онлайн-навчання</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Тестові та практичні завдання зі зворотним<br> зв'язком</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Роздатковий матеріал (корисні файли,<br> брошури, презентації)</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Клуб однодумців у Viber та підтримка <br>куратора</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Сертифікати після проходження <br>курсів</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Доступ до Бухгалтерської Відеоплатформи<br> №1:</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Відеокурси і вебінари<br>
(1100+ вже та 20+ щомісяця)</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Безлімітні швидкі консультації від експертів<br> (сервіс ОК)</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Бланки та зразки документів
<br>(2000+ вже та 30+ щомісяця)</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Консультант з пошуку та підготовки<br> документів (безлімітно, щодня)</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Калькулятори</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
                  <li class="flex justify-between items-center border-b border-gray-300 py-2">
                      <span>Довідники</span>
                      <div class="flex">
                          <img class="mr-64" src="~/assets/images/tick.png" alt="tick">
                          <img class="mr-28" src="~/assets/images/tick.png" alt="tick">
                      </div>
                  </li>
              </ul>
          </div>

      </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      targetDate: new Date('2023-10-03T17:00:00').getTime(),
      countdown: {
        hours: '00',
        minutes: '00',
        seconds: '00',
      },
    };
  },
  methods: {
    updateCountdown() {
      const currentDate = new Date().getTime();
      const timeDifference = this.targetDate - currentDate;

      if (timeDifference <= 0) {
        this.countdown.hours = '00';
        this.countdown.minutes = '00';
        this.countdown.seconds = '00';
        return;
      }

      const hours = Math.floor(timeDifference / (1000 * 60 * 60));
      const minutes = Math.floor((timeDifference % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((timeDifference % (1000 * 60)) / 1000);

      this.countdown.hours = hours.toString().padStart(2, '0');
      this.countdown.minutes = minutes.toString().padStart(2, '0');
      this.countdown.seconds = seconds.toString().padStart(2, '0');

      this.animateTimelineCircle(currentDate);
    },
    animateTimelineCircle(currentDate) {
      const timelineCircle = document.querySelector('.timeline-circle');
      const timelineItems = document.querySelectorAll('.base-timeline__item');

      const totalDuration = this.targetDate - new Date('2023-08-21T00:00:00').getTime();
      const elapsedDuration = currentDate - new Date('2023-08-21T00:00:00').getTime();
      const animationProgress = elapsedDuration / totalDuration;

      const containerWidth = timelineItems[timelineItems.length - 1].offsetLeft + timelineItems[timelineItems.length - 1].offsetWidth;
      const newPosition = containerWidth * animationProgress;

      timelineCircle.style.left = `${newPosition}px`;
    },
  },
  mounted() {
    this.updateCountdown();
    this.timerInterval = setInterval(this.updateCountdown, 1000);
  },
  beforeDestroy() {
    clearInterval(this.timerInterval);
  },
};
</script>

<style>
.base-timeline {
	list-style-type: none;
	position: relative;
	display: block;
	z-index: 2;
	width: 79%;
}

.base-timeline::before {
	content: '';
	width: 96%;
	border-top: 2px solid gray;
	display: block;
	position: absolute;
	top: 50%;
	z-index: -1;
}

.base-timeline__item {
	display: inline-block;
}

.base-timeline__item::before {
	margin-top: 1.5rem;
	display: block;
	content: '|';
	color: black;
}

.timeline-container {
	position: relative;
	width: 80%;
	display: flex;
	justify-content: center;
	align-items: center;
	margin: 0 auto;
}

.timeline-wrapper {
	position: relative;
	width: 100%;
}

.timeline-circle {
	position: absolute;
	background-color: yellow;
	border: 2px solid black;
	border-radius: 50%;
	width: 20px;
	height: 20px;
	left: 0;
	top: 50%;
	transform: translateY(-50%);
	transition: left 1s ease;
	z-index: 2;
}
</style>


