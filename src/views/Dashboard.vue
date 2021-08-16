<template>

  <div class="container-fluid main vh-100">
    <div class="row  justify-content-between align-items-center bg-light">
      <div class="col-3 col-lg-6">
        <nav class="navbar navbar-expand-lg navbar-light bg-light ">
          <div class="container-fluid">
            <a class="navbar-brand menu-control-laptop d-none d-lg-block" href="#">

              <i class="feather-align-left fs-2 menu-icon"></i></a>
            <a class="navbar-brand menu-control-phone d-block d-lg-none" href="#">
              <i class="feather-align-left fs-2 menu-icon"></i></a>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
              <form class="d-flex">
                <input class="form-control me-2" type="search" placeholder="Search projects..."
                       aria-label="Search">
              </form>
              <ul class="navbar-nav me-auto mb-2 mb-lg-0">

                <li class="nav-item dropdown">
                  <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button"
                     data-bs-toggle="dropdown" aria-expanded="false">
                    Mega Menu
                  </a>
                  <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                    <li><a class="dropdown-item" href="#">Action</a></li>
                    <li><a class="dropdown-item" href="#">Another action</a></li>
                    <li>
                      <hr class="dropdown-divider">
                    </li>
                    <li><a class="dropdown-item" href="#">Something else here</a></li>
                  </ul>
                </li>

              </ul>

            </div>
          </div>
        </nav>

      </div>
      <div class="col-9 col-lg-6">
        <div class="d-flex justify-content-end align-items-center fs-5">
          <i class="feather-message-circle menu-icon"></i>
          <i class="feather-bell-off menu-icon"></i>
          <img src="assets/img/us.png" class="img-fluid rounded-circle country-img" alt="">
          <img src="assets/img/profile.jpg" class="img-fluid rounded-circle profile-img" alt="">

          <ul class="navbar-nav me-3 mb-2 mb-lg-0">

            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown1" role="button"
                 data-bs-toggle="dropdown" aria-expanded="false">
                Ko Phyo
              </a>
              <ul class="dropdown-menu" aria-labelledby="navbarDropdown1">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li>
                  <hr class="dropdown-divider">
                </li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
              </ul>
            </li>

          </ul>

        </div>

      </div>
    </div>
    <div class="row px-3 px-lg-3 py-lg-4">
      <div class="col-12 col-lg-6 mt-3 mt-lg-0">

        <card1></card1>

      </div>
      <div class="col-12 col-lg-3 mt-3 mt-lg-0 d-flex flex-column justify-content-between">
        <Card2></Card2>

        <Card3></Card3>


      </div>
      <div class="col-12 col-lg-3 mt-3 mt-lg-0 d-flex flex-column ">

        <card4></card4>

        <card5></card5>

      </div>
    </div>
    <div class="row px-3 px-lg-3 py-lg-3">
      <div class="col-12 col-lg-3">
        <card6></card6>
      </div>
      <div class="col-12 col-lg-3">
        <Card7></Card7>
      </div>
    </div>
  </div>


</template>

<script>
import Card1 from "@/components/Card1";
import Card2 from "@/components/Card2";
import Card3 from "@/components/Card3";
import Card4 from "@/components/Card4";
import Card5 from "@/components/Card5";
import Card6 from "@/components/Card6";
import Card7 from "@/components/Card7";

export default {
  name: "Dashboard",
  components: {Card7, Card6, Card5, Card4, Card3, Card2, Card1},
}
</script>

<style scoped>

</style>