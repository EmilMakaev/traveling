<template>
  <div class="countries">
    <Country
      v-for="country in countries"
      v-bind="country"
      v-bind:key="country.title"
    />
  </div>
</template>

<script>
import Country from '@/components/Country'

export default {
  name: 'Countries',
  components: {
    Country
  },
  data() {
    return {
      countries: [
        {image: '687_anons-min_480_275_5_90.png', price: '118 112', title: 'Италия', name: 'Под небом Тосканы', destinations: 'Сансеполькро — (Перуджа) — Ассизи — Губбио — (Сиена) — Ла Верна — Ангиари — Монтерки — Ареццо — Кортона — (Пиенца) - (Монтепульчано)', duration: '8 дней / 7 ночей Русский язык 27.04.19 - 04.05.19 и еще 15 дат', extra: 'Авиаперелет включен!'},
        {image: '430_anons_480_275_5_90.png', price: '140 715', title: 'Исландия', name: 'Майские каникулы в Исландии', destinations: 'Рейкьявик — Тингвеллир — Гюдльфосс — Скафтафедль — Сельяландсфосс — Скоугафосс — Йёкюльсаурлоун — Голубая Лагуна — Снайфельсйёкутль — Arnarstapi — Рейкьявик', duration: '8 дней / 7 ночей Русский язык 27.04.19 - 04.05.19'},
        {image: '640anons_480_275_5_90.png', price: '37 302', title: 'Турция', name: 'Открытие Турции', destinations: 'Стамбул — Анкара — Каппадокия — Конья — Памуккале — Эфес — Кушадасы — Пергам — Ассос — Троя — Стамбул', duration: '8 дней / 7 ночей Русский язык 28.04.19 - 05.05.19и еще 3 даты'},
        {image: '117_anons-min_480_275_5_90.png', price: '145 000', title: 'Норвегия, Шпицберген', name: 'От Свальбарда до Груманта', duration: '8 дней / 7 ночей Русский язык 27.04.19 - 04.05.19и еще 15 дат', extra: 'Гарантированный тур!'}
      ]
    }
  }
}
</script>