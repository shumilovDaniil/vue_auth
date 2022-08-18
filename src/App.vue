<style src="./assets/styles/tailwind.css" />

<template>
  <div class="login__page">
    <div class="login__window">
      <form class="form" action="" method="post">
        <div class="form__fields">
          <div class="form__login form_row">
            <v-label label="Логин" class="form_row__label" for="user__login"/>
            <v-input type="text" placeholder="Введите логин" class="form__input" name="user__login" />
          </div>
          <div class="form__password form_row">
            <v-label label="Пароль" class="form_row__label" for="user__password"/>
            <v-input type="password" placeholder="Введите пароль" class="form__input" name="user__password" />
          </div>
        </div>
        <nav class="form__nav">
          <ul>
            <li><a href="#">Создать аккаунт</a></li>
            <li><a href="#">Забыли пароль?</a></li>
          </ul>
        </nav>
      </form>
    </div>
    <div class="login__btns">
      <blueBtn label="Войти" />
      <blueLink label="На главную" />
    </div>
  </div>
</template>

<script>
import blueBtn from "./components/ui/blue-btn.vue";
import blueLink from "./components/ui/blue-link.vue";
import vInput from "./components/ui/v-input.vue";
import vLabel from "./components/ui/v-label.vue";

export default {
  name: "app",
  components: {
    blueBtn,
    blueLink,
    vInput,
    vLabel
  }
};
</script>


<style lang="scss">

.login__page {
  margin: 154px auto 0;
  max-width: 501px;
  padding: 0 10px;
}

.login__window {
  padding: 30px;
  background: #FDFDFE;
  border: 1px solid #E2E3ED;
  box-shadow: 0px 0px 30px rgba(170, 173, 178, 0.25);
  border-radius: 12px;
  margin-bottom: 30px;
}

.form__fields {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.form__login, .form__password {
  display: flex;
  flex-direction: column;
}

.form__input {
  padding: 17px 23px;
  background: #FAFAFC;
  border: 1px solid #E2E3ED;
  border-radius: 12px;
  font-weight: 400;
  font-size: 12px;
  line-height: 188.7%;
}

.form_row__label {
  font-size: 14px;
  line-height: 17px;
  letter-spacing: 0.03em;
  margin-bottom: 10px;
  color: #222431;
}

.form__nav {
  ul {
    color: #72768F;
    display: flex;
    justify-content: space-between;
    margin-top: 15px;
  }

  li {
    font-weight: 500;
    font-size: 12px;
    line-height: 188.7%;
  }
}

.login__btns {
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  align-items: center;


  @media (max-width: 410px) {
    justify-content: center;
  }

}

</style>



