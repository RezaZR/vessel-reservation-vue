<template lang="pug">
  div
    HeaderMain
    Headline
    Information
    Join
    Trivia
</template>

<script>
import HeaderMain from "@/components/HeaderMain";
import Headline from "@/components/Headline";
import Information from "@/components/Information";
import Join from "@/components/Join";
import Trivia from "@/components/Trivia";

export default {
  name: "home",
  components: { HeaderMain, Headline, Information, Join, Trivia }
};
</script>
