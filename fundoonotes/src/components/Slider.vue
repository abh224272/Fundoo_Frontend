<template>
  <div class="drawer">
    <v-navigation-drawer
      height="100%"
      width="180"
      hide-overlay
      expand-on-hover
      permanent
      >
      <v-list
        nav
        dense
      >
      <v-list-item link to="/dashboard/notes">
        <v-list-item-icon>
          <v-icon>mdi-lightbulb</v-icon>
          </v-list-item-icon>
            <v-list-item-title>Notes</v-list-item-title>
          </v-list-item>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-alert</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Reminders</v-list-item-title>
          </v-list-item>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-pencil</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Edit Labels</v-list-item-title>
          </v-list-item>
          <v-list-item link to="/dashboard/archive">
            <v-list-item-icon>
              <v-icon>mdi-archive</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Archive</v-list-item-title>
          </v-list-item>
          <v-list-item link to="/dashboard/trash">
            <v-list-item-icon>
              <v-icon>mdi-delete</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Trash</v-list-item-title>
          </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
    methods:{
        closeNav: function() {
            document.getElementById("mySidenav").style.width = "0";
        }
    }
}
</script>

<style scoped>
.drawer{
  height: 100vh;
}
.v-list-item--active{
  background: #FEEFC3;
}
</style>