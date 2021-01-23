<template>
  <form class="form">
    <h2 class="form__title">Register <span>New Account</span></h2>

    <label for="fullName" class="form__label">Full Name</label>
    <input type="text" name="fullName" class="form__input">

    <label for="email" class="form__label">Email Adress</label>
    <input type="email" name="email" class="form__input">

    <label for="phone" class="form__label">Phone Number</label>
    <input type="telephone" name="phone" class="form__input">

    <div class="form__row">
      <div class="form__cal">
        <label for="pass" class="form__label">Password</label>
        <input type="password" name="pass" class="form__input">
      </div>

      <div class="form__cal">
        <label for="passR" class="form__label">Repeat Password</label>
        <input type="password" name="passR" class="form__input">
      </div>
    </div>

    <div class="form__row">
      <div class="form__cal">
        <p class="form__signIn">Do you already have an account? <a href="#">Sign In</a></p>
      </div>
      <div class="form__cal">
        <button type="submit" class="form__button">Create account and continue</button>
      </div>
    </div>
    
  </form>
</template>

<script>

</script>

<style lang="scss" scoped>
.form {
  display: flex;
  flex-direction: column;
  width: 600px;
  font-weight: normal;
  background: #1B202A;
  color: #FAF9FE;
  border: none;
  border-radius: 20px;
  margin-top: 160px;
  padding: 28px;

  // .from__title
  &__title {
    font-weight: normal;
    span {
      font-weight: bold;
      color: #B1B1FF;
    }
  }

  // .form__label
  &__label {
    font-size: 14px;
    display: inline-block;
    margin-bottom: 6px;
    color: #A5ACB5;
  }

  // .form__input
  &__input {
    background: #1C1F2C;
    color: #FAF9FE;
    border: 2px solid #262F3A;
    border-radius: 6px;
    font-size: 16px;
    width: 100%;
    margin-bottom: 16px;
    padding: 12px 14px;
    box-sizing: border-box;

    // &:-webkit-autofill { 
    //   -webkit-background-clip: text;
    // }
}
  
  // .form__row
  &__row {
    display: flex;
    justify-content: space-between;
  }

  // .form__cal
  &__cal {
    width: 48%;
  }

  // .form__signIn
  &__signIn {
    box-sizing: border-box;
    font-size: 14px;
    letter-spacing: 0.05em;
    margin: 0;
    padding: 12.05px 14px;
    border: 2px solid #262F3A;
    border-radius: 6px;
    color: #A5ACB5;
    a {
      text-decoration: none;
      color: #FAF9FE;
    }
  }

  // .from__button
  &__button {
    background-image: linear-gradient(to right, #128AAB, #24BBB4);
    color: #FAF9FE;
    font-size: 16px;
    border: none;
    border-radius: 6px;
    width: 100%;
    padding: 14px 14px;
  }
}

</style>