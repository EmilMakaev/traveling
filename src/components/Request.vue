<template>
  <div class="request">
    <h3 class="request__title">Заявка на подбор путешествия</h3>
    <div class="request__you">
      <div>
        <p>ИМЯ <span class="required-fields">*</span></p>
        <input class="input-contacts" type="text" placeholder="Ваше имя">
      </div>
      <div>
        <p>ТЕЛЕФОН <span class="required-fields">*</span></p>
        <input class="input-contacts" placeholder="+7___ ___ __ __" type="number">
      </div>
    </div>
    <div class="request__trip">
      <div>
        <p>КУДА И КОГДА ХОТИТЕ ПОЕХАТЬ?</p>
        <input class="input-contacts" type="text" placeholder="Континент, страна или город">
      </div>
      <div>
        <p>КОГДА?</p>
        <input class="input-contacts" type="number" placeholder="Даты или временной интервал">
      </div>
    </div>

    <div class="additional-verification">
      <input class="additional-verification__input" type="checkbox" id="offers" value="Получать предложения">
      <label for="offers">Получать свежие предложения по электронной почте</label>
    </div>
    <p>Каждую неделю мы делаем для вас обзор лучших экспедиций, статей и лайфхаков для путешественников. Если вдруг вам не понравится, вы сможете отписаться в любой момент.</p>
    
    <div class="additional-verification">
      <input class="additional-verification__input" type="checkbox" id="data" value="Персональные данные">
      <label for="data">С обработкой своих персональных данных согласен.</label>
    </div>

    <p>Отправляя заявку я подтверждаю согласие с условиями Пользовательского соглашения</p>
    <br>
    <p><span class="required-fields">*</span> Поля, которые надо обязательно заполнить</p>

    <button class="btn btn-main">Отправить</button>
  </div>
</template>

<script>
export default {
  name: 'Request'
}
</script>