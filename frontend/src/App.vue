<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <nav className='navbar'>
        <div className="container flex">
            <ul className="flex navbar-nav">
            <div className="router-links">
                <RouterLink className="nav-link" to="/">Home</RouterLink>
                <RouterLink className="nav-link" to="/Categories">Categories</RouterLink>
                <RouterLink className="nav-link" to="/Products">Products</RouterLink>
                <RouterLink className="nav-link" to="/Contacts">Contacts</RouterLink>
            </div>
                </ul>
                  </div>               
    </nav>
  <RouterView />
</template>

<style scoped>
.flex {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-left: 30px;
}
.navbar {
  position: fixed;
  width: 100%;
  top: 0;
  left: 0;
  background-color: #cc0000;
  color: white;
  font-family: 'Exo 2', sans-serif;
  padding: 1em;
}

.router-links {
text-align:center;
}

.navbar-nav {
  list-style: none;
  gap: 32px;
  font-size: 14px;
}
.nav-link {
  text-decoration: none;
  color: white;
  padding: 16px;
  display: inline-block;
}
.nav-link:hover {
  background-color: #6b869c;
}
.nav-link:nth-child(1) {
  margin-left: -16px;
}
.nav.link.active {
  text-decoration: underline;
  color: white;
}
.login-btn {
  margin-right: 30px;
  border: 0;
  padding: 16px;
  background-color: #7997af;
  color: white;
  cursor: pointer;
  font-family: "Roboto Mono", monospace;
}
.login-btn:hover {
  background-color: #6b869c;
}


.avatar-dropdown {
  position: relative;
}
.avatar {
  margin-right: 15px;
  border-radius: 50%;
  overflow: hidden;
  height: 35px;
  cursor: pointer;
}
img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.dropdown {
  position: absolute;
  width: 150px;
  background-color: white;
  padding: 8px;
  box-shadow: 2px 2px 6px black;
  border-radius: 4px;
  right: 0;
  bottom: -8px;
  transform: translateY(100%);
}
.logout-btn {
  width: 100%;
  padding: 8px;
  border: 0;
  border-radius: 8px;
  background-color: #7997af;
  color: white;
  text-transform: uppercase;
  font-weight: 600px;
  cursor: pointer;
}

.logout-btn:hover {
  background-color: #3e4e5a;
}

.logout-btn:active {
  background-color: #5fa6e0;
}

</style>
