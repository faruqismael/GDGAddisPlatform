<template>
  <v-card color="white" height="60px" class="white hidden-sm-and-up" flat>
    <v-bottom-nav :active.sync="bottomNav" :value="true" app color="white" class="elevation-2">
      <v-btn color="#518FF5" flat value="Home" router to="/home">
        <span>Home</span>
        <v-icon>dashboard</v-icon>
      </v-btn>

      <v-btn color="#518FF5" flat value="events" router to="/events">
        <span>Events</span>
        <v-icon>mdi-calendar</v-icon>
      </v-btn>

      <v-btn color="#518FF5" flat value="team" router to="/team">
        <span>Team</span>
        <v-icon>group</v-icon>
      </v-btn>

      <v-btn color="#518FF5" flat value="about" router to="/about">
        <span>About</span>
        <v-icon>mdi-information-outline</v-icon>
      </v-btn>

      <v-btn color="#518FF5" flat value="wtmaddis" router to="/wtmaddis">
        <span>WTMAddis</span>
        <v-icon>mdi-human-female-female</v-icon>
      </v-btn>

      <v-btn color="#518FF5" flat value="contact" router to="/contact">
        <span>Contact</span>
        <v-icon>mdi-account-box-outline</v-icon>
      </v-btn>

      <!-- <v-btn
        color="#518FF5"
        flat
        value="contact"
        router
        to="/contact"
      >
        <span>Contant</span>
        <v-icon>person</v-icon>
      </v-btn>-->
    </v-bottom-nav>
  </v-card>
</template>


<script>
export default {
  data() {
    return {
      bottomNav: "recent",
      items: [
        { title: "Home", icon: "dashboard", route: "/home" },
        {
          title: "Attending",
          icon: "mdi-account-check-outline",
          route: "/attending"
        },
        { title: "Sessions", icon: "mdi-code-braces", route: "/sessions" },
        {
          title: "Speakers",
          icon: "mdi-microphone-outline",
          route: "/speakers"
        }
      ]
    };
  }
};
</script>