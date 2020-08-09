<template>
  <div>
    <div class="login">
      <div class="login-image">
        <!-- <h1>Image</h1> -->
        <img src="@/assets/images/model.png" alt />
      </div>
      <div class="login-form">
        <div class="form">
          <h2>Create your free account</h2>
          <p>
            Already registered?
            <a href="#">Sign in</a>
          </p>
          <div class="form-card">
            <div class="names">
              <div class="form-gap lastname">
                <label for="firstName">First Name</label>
                <br />
                <div class="form-field">
                  <input type="text" name id="firstName" />
                  <svg xmlns="http://www.w3.org/2000/svg" width="16" height="18" viewBox="0 0 16 18" fill="none">
                    <path
                      d="M15 16.75V15C15 13.067 13.433 11.5 11.5 11.5H4.5C2.567 11.5 1 13.067 1 15V16.75"
                      stroke="#013C61"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M8 8C9.933 8 11.5 6.433 11.5 4.5C11.5 2.567 9.933 1 8 1C6.067 1 4.5 2.567 4.5 4.5C4.5 6.433 6.067 8 8 8Z"
                      stroke="#013C61"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </div>
                <hr />
              </div>
              <div class="form-gap lastname">
                <label for="lastName">Last Name</label>
                <br />
                <div class="form-field">
                  <input type="text" name id="lastName" />
                  <svg xmlns="http://www.w3.org/2000/svg" width="16" height="18" viewBox="0 0 16 18" fill="none">
                    <path
                      d="M15 16.75V15C15 13.067 13.433 11.5 11.5 11.5H4.5C2.567 11.5 1 13.067 1 15V16.75"
                      stroke="#013C61"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M8 8C9.933 8 11.5 6.433 11.5 4.5C11.5 2.567 9.933 1 8 1C6.067 1 4.5 2.567 4.5 4.5C4.5 6.433 6.067 8 8 8Z"
                      stroke="#013C61"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </div>
                <hr />
              </div>
            </div>
            <div class="email">
              <label for="email">Email</label>
              <br />
              <div class="form-field">
                <input type="email" name id="mail" />
                <svg xmlns="http://www.w3.org/2000/svg" width="17" height="17" viewBox="0 0 17 17" fill="none">
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M8.14328 11.0002C9.72123 11.0002 11.0004 9.72105 11.0004 8.14309C11.0004 6.56514 9.72123 5.28595 8.14328 5.28595C6.56532 5.28595 5.28613 6.56514 5.28613 8.14309C5.28613 9.72105 6.56532 11.0002 8.14328 11.0002Z"
                    stroke="#013C61"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M11.0004 5.28596V8.85739C11.0004 10.0409 11.9598 11.0003 13.1433 11.0003C14.3267 11.0003 15.2861 10.0409 15.2861 8.85739V8.14311C15.2859 4.82375 12.9991 1.94198 9.76659 1.18761C6.5341 0.433237 3.20791 2.0051 1.73846 4.98148C0.269016 7.95786 1.0436 11.5543 3.60801 13.6619C6.17243 15.7695 9.85078 15.8327 12.4861 13.8145"
                    stroke="#013C61"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </div>
              <hr />
            </div>
            <div class="password">
              <label for="email">Password</label>
              <br />
              <div class="form-field">
                <input type="password" name id="password" />
                <svg xmlns="http://www.w3.org/2000/svg" width="19" height="15" viewBox="0 0 19 15" fill="none">
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M1 7.54545C1 7.54545 4.27273 1 10 1C15.7273 1 19 7.54545 19 7.54545C19 7.54545 15.7273 14.0909 10 14.0909C4.27273 14.0909 1 7.54545 1 7.54545Z"
                    stroke="#013C61"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M10 10C11.3556 10 12.4546 8.9011 12.4546 7.54549C12.4546 6.18988 11.3556 5.09094 10 5.09094C8.64441 5.09094 7.54547 6.18988 7.54547 7.54549C7.54547 8.9011 8.64441 10 10 10Z"
                    stroke="#013C61"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </div>
              <hr />
            </div>
            <router-link to="/home">
              <div class="button">
                <input class="submit" type="button" value="Continue" />
              </div>
            </router-link>
          </div>
        </div>
        <div class="footer">
          <p>
            By signing up, you agree to our
            <a href="#">Terms</a> and
            <a href="#">Privacy Policy</a>
          </p>
          <p>© 2019 Tinylabs. All rights reserved</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      name: "hello",
    };
  },
};
</script>
<style scoped>
/* * {
  --primary-color: #013c61;
  --font-color: #6a7e8a;
  --green: #2bda53;
} */
body {
  padding: 0;
  margin: 0;
}
p,
h2 {
  /* text-align: center; */
  color: var(--primary-color);
}
a {
  color: var(--green);
}
label {
  color: (var(--font-color));
}
.login {
  display: flex;
  /* min-height: 100vh; */
}
.login-image {
  width: 45%;
  /* background-color: green; */
  min-height: 100vh;
  background-image: url("/assets/images/model.png");
  background-size: cover;
}
.login-form {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  color: black;
  width: 55%;
  position: relative;
}
img {
  height: 100%;
  width: 100%;
}
.form-card {
  background: #ffffff;
  box-shadow: 0px 20px 50px #eaeee9;
  border-radius: 5px;
  padding: 3rem;
  margin-top: 2rem;
}
input {
  border: none;
  outline: none;
  padding: 0.5rem;
  width: 100%;
}
.form-field {
  display: flex;
  justify-content: space-between;
}
.names {
  display: flex;
}
.form-gap {
  margin: 0 1rem;
}
hr {
  border: 0.02rem solid #d8d8d8;
  margin: 0;
}
.password,
.email {
  margin: 2rem 1rem;
}
.button {
  display: flex;
}
.submit {
  margin-left: auto;
  padding: 1rem;
  width: 40%;
  background-color: #2bda53;
  color: white;
  box-shadow: 0px 7px 15px rgba(43, 218, 83, 0.2);
  border-radius: 3px;
  cursor: pointer;
}
.footer {
  position: absolute;
  bottom: 0;
  display: flex;
  justify-content: space-evenly;
  width: 100%;
}
@media only screen and (max-width: 768px) {
  .login-image {
    display: none;
  }
  .login-form {
    width: 90%;
    margin: auto;
    flex-direction: column;
  }
  .form-card {
    padding: 1rem;
    /* width: 100%; */
    /* margin: auto; */
  }
  .submit {
    width: 100%;
  }
  .names {
    flex-direction: column;
  }
  .password,
  .email {
    margin: 2rem 0.5rem;
  }
  .form {
    width: 100%;
  }
  .lastname {
    margin: 2rem 0.5rem 0 0.5rem;
  }
  .login {
    background-color: #f6f8f8;
  }
  h2,
  p {
    text-align: center;
  }
  .footer {
    position: relative;
    /* flex-direction: column;
    text-align: center;
    margin-top: 0.5rem; */
    display: block;
    margin-top: 0.5rem;
  }
  .footer p {
    font-size: 0.7rem;
  }
}
</style>
