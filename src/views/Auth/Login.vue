<template>
  <form class="card auth-card">
    <div class="card-content">
      <span class="card-title">Вход</span>
      <div class="input-field">
        <input type="text" id="username" class="validate">
        <label for="username">Введите имя пользователя:</label>
        <small class="helper-text invalid">failure</small>
      </div>
      <div class="input-field">
        <input type="password" id="password" class="validate">
        <label for="password">Введите пароль:</label>
        <small class="helper-text invalid">failure</small>
      </div>
      <div class="card-action">
        <div>
          <button
                  class="btn waves-effect waves-light auth-submit"
                  type="submit"
          >
            Войти
            <i class="material-icons right">send</i>
          </button>
        </div>
        <p class="center">
          Если у вас нет аккаунта?
          <router-link href="/">Зарегистрировать</router-link>
        </p>
      </div>
    </div>
  </form>
</template>