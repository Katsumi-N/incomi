<template>
  <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand to="/" nuxt>インコミ</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item to="/" nuxt>Home</b-nav-item>
        <b-nav-item to="/mypage" nuxt>My page</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template v-slot:button-content>
            <em>User</em>
          </template>
          <b-dropdown-item to="/mypage" nuxt>My page</b-dropdown-item>
          <b-dropdown-item to="/login" nuxt>login</b-dropdown-item>
          <b-dropdown-item to="/signup" nuxt>signup</b-dropdown-item>
          <b-dropdown-item to="/" nuxt>signout</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>
