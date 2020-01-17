<template>
  <div id="app">
    <div id="nav">
      <router-link to="/"> Orange University </router-link> |
      <router-link to="/"> Home </router-link> |
      <router-link to="/about"> About </router-link> |
      <router-link to="/students"> Students </router-link> |
      <router-link to="/courses"> Courses </router-link> | 
      <router-link to="/instructors"> Instructors </router-link> | 
      <router-link to="/departments"> Departments </router-link> | 
      <router-link to="/training_centers"> Training Centers </router-link> | 
      <router-link to="/search"> Search </router-link><br><br> |
      <a href="https://orangeuniversitytest.b2clogin.com/orangeuniversitytest.onmicrosoft.com/b2c_1_siupin/oauth2/v2.0/authorize?client_id=86354b0a-9342-47f5-b30c-8c21d16b56ed&redirect_uri=https%3A%2F%2Forangeuniversity-dev.azurewebsites.net%2Fsignin-oidc&response_type=id_token&scope=openid%20profile&response_mode=form_post&nonce=637148723765070161.YmI5N2Y4ODQtYzhjNi00YmFlLTkxNDAtY2ZiMGI0YmYyODY0M2I5MmNjZTUtZjg2NC00MGJiLWJhMTAtMDJhMTYxYzM3MWY4&state=CfDJ8HEQhORTJXxAjliUey7N2va8eRQq6KP3bRE9UqqOyc-5fGWNlnKF0SwexapFihr53W3r-ccHG-uz1EFFiEJSCq3FfACgiNgsozPfi6X9Lc1RGwnsKHdcOICnDOg6TZIw0yvbB4zUTKbZS1rtOmduvbPKT5BYi0aSpv2kPeoWIjgvexTTUbwE0G6yFN64NCT6iqwASpNJ5sNkQF5wAgWvm3LNZCrcYla6-3TJC0wlKJP-Tgnv9KlKSxAjoFqjj4nuNPefKg4kAyNOljLaNP2I0mXQx-RxaPjNWW73I3IuegFxF4CHyTeZieRL9iskTjzSzEfQkwjq1i4wg3jQMP2qcoY&x-client-SKU=ID_NETSTANDARD2_0&x-client-ver=5.3.0.0" to="/sign_in"> Sign in </a> | 
      <a href="https://orangeuniversitytest.b2clogin.com/orangeuniversitytest.onmicrosoft.com/B2C_1_SiUpIn/api/CombinedSigninAndSignup/unified?local=signup&csrf_token=TnVTbURzQnU2cFBLbFdZeU5vNFc0MmpLMzV6VVNVTTJHZkNVbjBXUm8zaVo4VlJmeVJ6WEZ0ZXlLQXNwVmcrZnp1UkJLTkhFOW1SRmFwVXp0dWM2OFE9PTsyMDIwLTAxLTE3VDE1OjQwOjIxLjMwNDU3MzZaO056R1dNNmduejJ1K3NDZVRJd1BZUXc9PTt7Ik9yY2hlc3RyYXRpb25TdGVwIjoxfQ==&tx=StateProperties=eyJUSUQiOiIxZmE0MzEwMS05YWNiLTQ1ZjctYTdlMS01OWFmZDdlMjdiZjgifQ&p=B2C_1_SiUpIn" to="/sign_up"> Sign up </a>
    </div>
    <router-view/>
  </div>
</template>

<style>
body{
  background: url(../public/background.jpg) no-repeat center center fixed; 
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
a{
    text-decoration: none;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #f7f7f7;
  background-color:black;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #ffffff;
}

#nav a.router-link-exact-active {
  color: #ffa500;
}
</style>
