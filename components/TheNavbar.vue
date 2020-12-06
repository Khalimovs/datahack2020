<template>
    <div class="width-1920">
      <b-navbar toggleable="lg" >
        <b-navbar-brand to="/">
            <img src="@/assets/img/logo.svg" alt="LOGO">
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="mx-auto">
            <b-nav-item class="mx-3" to="/">LatestEvents</b-nav-item>
            <b-nav-item class="mx-3" to="/">Categories</b-nav-item>
            <b-nav-item class="mx-3" to="/">Teams</b-nav-item>
          </b-navbar-nav>
          <b-navbar-nav class="ml-auto">
            <b-button variant="primary">Log in</b-button>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
</template>