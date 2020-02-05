<template style="background: #D1C4E9">
  <v-row >
    <v-col>
      <v-sheet style="background: #D1C4E9">
        <v-calendar
          color="#D1C4E9"
          type="day"
        >
          <template clolor="#D1C4E9" v-slot:day-header="{ present }">
            <template
              v-if="present"
              class="text-center"
            >
              Today
            </template>
          </template>

          <template v-slot:interval="{ hour }">
            <div
              class="text-center"
            >
              {{ hour }} o'clock
            </div>
          </template>
        </v-calendar>
      </v-sheet>
    </v-col>
  </v-row>
</template>
<script>
  export default {
    data: () => ({}),
  }
</script>