<template>

  <div class="d-flex pt-2">
    <div class="_backdrop fade"></div>
    <SideBar></SideBar>
    <router-view>

    </router-view>


  </div>


</template>

<script>


import SideBar from "@/components/SideBar";

export default {
  name: "app",
  components: {SideBar},
}

</script>

<style lang="scss">
$primary:#5A8DEE;
$progress-height: 0.4rem;
@import "~bootstrap";

@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800;900&display=swap");


* {
  font-family: 'Poppins', sans-serif;
}
.rounded-circle{
  line-height: 40px;
}

.sidebar {

  width: 14%;
  transition: 0.5s;

}

.main {


  width: 100%;
  overflow-y: scroll;
}

.menu {
  position: fixed;
  top: 0;
  z-index: 2000;
  width: 100%;

  background-color: #0a31be;
}

.country-img {
  width: 22px;
  height: 22px;
  margin-right: 20px;
}

.profile-img {
  width: 30px;
  height: 30px;
  margin-right: 20px;
}

.menu-icon {
  margin-right: 20px;
  transition: 0.2s;

}

.menu-icon:hover {
  color: var(--bs-primary);
  cursor: pointer;
}

.menu-btn{
  width: 100%;
}
.menu-btn:focus {
  border-color: transparent;
  box-shadow: none;
}

.nav-brand {
  fill: var(--bs-primary);
}

p, h2, a {
  font-size: 0.9rem;
}

.close {
  margin-left: -20%;


}

.full-width {
  width: 100%;

}

@media screen and (max-width: 576px) {
  .sidebar {
    position: fixed;
    left: 0;
    top: 0;
    margin-left: -100%;
    z-index: 2000;
    transition: 0.5s ease-in-out;
  }

  .sidebar.open {
    margin-left: 0;
    width: 250px;
  }

  .main {
    width: 100%;
  }

  .menu-icon {
    margin-right: 10px;
    transition: 0.2s;

  }
  .menu-icon:hover {
    color: var(--bs-primary);
    cursor: pointer;
  }
  .profile-img {
    width: 25px;
    height: 25px;

    margin-right: 10px;
  }

  .country-img {
    margin-right: 10px;
  }


}


</style>