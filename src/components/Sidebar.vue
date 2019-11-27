<template lang="pug">
  .sidebar
    .container-fluid
      .row
        .col-md-12
          .sidebar__logo 
            a(href="#") LOGO
          .sidebar__content
            .sidebar__content__list.active
              a(href="#")
                p Dashboard
                span
            .sidebar__content__list
              a(href="#")
                p User Management
                span
            .sidebar__content__list 
              a(href="#")
                p Feeds
                span
            .sidebar__content__list 
              a(href="#")
                p My Vessels
                span
            .sidebar__content__list 
              a(href="#")
                p Fleet Request
                span
            .sidebar__content__list 
              a(href="#")
                p Transactions
                span
            .sidebar__content__list 
              a(href="#")
                p Coins &#38; Balance
                span
            .sidebar__content__list 
              a(href="#")
                p Help
                span
            .sidebar__content__list 
              a(href="#")
                p Settings
                span
            .sidebar__content__list 
              a(href="#")
                p Log Out
                span
</template>

<script>
export default {
  name: "sidebar"
};
</script>