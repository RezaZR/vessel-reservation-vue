<template lang="pug">
  .header.header--main
    .container-xl
      .row
        .col-md-3
          router-link(to="/").header__logo LOGO
        .col-md-9
          .header__navigation
            .header__navigation__list.active
              router-link(to="/") Home
            .header__navigation__list 
              router-link(to="/our_company") Our Company
            .header__navigation__list 
              router-link(to="/help") Help
            button.header__navigation__list.header__navigation__list--dropdown.button.button--transparent.button--dropdown#dropdown_language(@click="handleClickDropdown()") {{ activeLanguage }}
              .dropdown(v-if="isDropdownActive")
                ul
                  li English
                  li Bahasa Indonesia
            button.header__navigation__list.button.button--white.button--radius-25 Log in
            button.header__navigation__list.button.button--black.button--radius-25 Sign up
</template>

<script>
export default {
  name: "header_main",
  data() {
    return {
      isDropdownActive: false,
      activeLanguage: "English"
    };
  },
  mounted() {
    // this.spawnDropdown();
  },
  methods: {
    // spawnDropdown() {
    //   var button = document.querySelector("#dropdown_language");

    //   var dropdownElement = document.createElement("div");
    //   dropdownElement.classList.add("dropdown");

    //   button.insertAdjacentElement("afterend", dropdownElement);

    //   var ul = document.createElement("ul");
    //   dropdownElement.appendChild(ul);

    //   var firstList = document.createElement("li");
    //   firstList.innerHTML = "English";
    //   ul.appendChild(firstList);

    //   var secondList = document.createElement("li");
    //   secondList.innerHTML = "Bahasa Indonesia";
    //   ul.appendChild(secondList);
    // },
    handleClickDropdown() {
      this.isDropdownActive = !this.isDropdownActive;
    }
  }
};
</script>