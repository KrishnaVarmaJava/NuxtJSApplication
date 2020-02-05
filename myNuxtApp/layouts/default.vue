<template>
<div>
    <v-card
    color="grey lighten-4"
    flat
    height="100px"
    tile
  >
    <v-toolbar style="background: #673AB7" dense >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title >Title</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
      <template v-slot:extension>
        <v-tabs color="#BA68C8" grow="true" align-with-title>
          <v-tab to='/'>Profile</v-tab>
          <v-tab to='/timesheet'>Time Sheet</v-tab>
          <v-tab to='/leaves'>Leaves</v-tab>
          <v-tab to='/claims'>Claims</v-tab>
          <v-tab to='/payslip'>Pay Slips</v-tab>
        </v-tabs>
      </template>
      <v-sheet
      id="scrolling-techniques-3"
      class="overflow-y-auto"
    >
    </v-sheet>
    </v-toolbar>
    
  </v-card>
      
  <nuxt/>
</div>
</template>
<script>
  export default {
    data: () => ({
      items: [
        { title: 'Click Me' },
        { title: 'Click Me' },
        { title: 'Click Me' },
        { title: 'Click Me 2' },
      ],
    }),
  }
</script>