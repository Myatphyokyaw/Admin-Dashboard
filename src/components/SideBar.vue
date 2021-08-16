<template>
  <div class="sidebar">

    <div class=" vh-100 bg-white">

      <a class="navbar-brand" href="#">

        <div class="d-flex justify-content-center align-items-center py-3">
          <svg version="1.1" class="nav-brand" xmlns="http://www.w3.org/2000/svg"
               xmlns:xlink="http://www.w3.org/1999/xlink" x="0px"
               y="0px" width="20px" height="20px" viewBox="0 0 20 20" enable-background="new 0 0 20 20"
               xml:space="preserve">
            <path d="M19.4,4.1l-9-4C10.1,0,9.9,0,9.6,0.1l-9,4C0.2,4.2,0,4.6,0,5s0.2,0.8,0.6,0.9l9,4C9.7,10,9.9,10,10,10s0.3,0,0.4-0.1l9-4
              C19.8,5.8,20,5.4,20,5S19.8,4.2,19.4,4.1z"></path>
            <path d="M10,15c-0.1,0-0.3,0-0.4-0.1l-9-4c-0.5-0.2-0.7-0.8-0.5-1.3c0.2-0.5,0.8-0.7,1.3-0.5l8.6,3.8l8.6-3.8c0.5-0.2,1.1,0,1.3,0.5
              c0.2,0.5,0,1.1-0.5,1.3l-9,4C10.3,15,10.1,15,10,15z"></path>
            <path d="M10,20c-0.1,0-0.3,0-0.4-0.1l-9-4c-0.5-0.2-0.7-0.8-0.5-1.3c0.2-0.5,0.8-0.7,1.3-0.5l8.6,3.8l8.6-3.8c0.5-0.2,1.1,0,1.3,0.5
              c0.2,0.5,0,1.1-0.5,1.3l-9,4C10.3,20,10.1,20,10,20z"></path>
          </svg>
          <h5 class="text-dark ms-3">AppStack</h5>
        </div>

      </a>

<!--      <div class="accordion accordion-flush" id="accordionFlushExample">-->

<!--        <div class="accordion-item bg-transparent text-muted">-->
<!--          <h2 class="accordion-header" id="flush-headingOne">-->

<!--            <div class="px-3">-->
<!--              <p class="m-0">Pages</p>-->
<!--            </div>-->


<!--            <button class="accordion-button collapsed bg-transparent text-dark accordion-btn" type="button"-->
<!--                    data-bs-toggle="collapse"-->
<!--                    data-bs-target="#flush-collapseOne" aria-expanded="false"-->
<!--                    aria-controls="flush-collapseOne">-->
<!--              <p class="m-0">-->
<!--                Dashboards-->
<!--              </p>-->
<!--            </button>-->
<!--          </h2>-->
<!--          <div id="flush-collapseOne" class="accordion-collapse collapse" aria-labelledby="flush-headingOne"-->
<!--               data-bs-parent="#accordionFlushExample">-->
<!--            <div class="accordion-body py-0 px-4">-->

<!--              <div class="list-group ">-->
<!--                <router-link href="#" class="list-group-item list-group-item-action border-0 text-muted"-->
<!--                   aria-current="true">-->
<!--                  Default-->
<!--                </router-link>-->
<!--                <router-link href="#" class="list-group-item list-group-item-action border-0 text-muted"-->
<!--                   aria-current="true">-->
<!--                  Analytics-->
<!--                </router-link>-->
<!--                <router-link href="#" class="list-group-item list-group-item-action border-0 text-muted"-->
<!--                   aria-current="true">-->
<!--                  Social-->
<!--                </router-link>-->
<!--                <router-link href="#" class="list-group-item list-group-item-action border-0 text-muted"-->
<!--                   aria-current="true">-->
<!--                  Crypto-->
<!--                </router-link>-->

<!--              </div>-->
<!--            </div>-->
<!--          </div>-->
<!--        </div>-->

<!--      </div>-->
      <div>
        <router-link :to="{name:'Dashboard'}" class="btn menu-btn">Dashboard</router-link>
        <router-link :to="{name:'About'}" class="btn menu-btn">About</router-link>
      </div>




    </div>

  </div>
</template>

<script>
export default {
  name: "SideBar"
}
</script>

<style scoped>

</style>