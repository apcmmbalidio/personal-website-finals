<template>
  <card class="card" title="Education List">
    <div>
      <ul class="list-unstyled education-list">
        <li v-for="education in educationList" :key="education.level">
          <div class="row">
            <div class="col-12">
              <strong>{{ education.level }}</strong>
              <br />
              <small>{{ education.institution }}</small>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </card>
</template>

<script>
export default {
  data() {
    return {
      educationList: [
        {
          level: "Primary Education",
          institution: "Rancho Imperial Learning Center",
        },
        {
          level: "Secondary Education",
          institution: "Tagaytay City Science National High School - ISHS",
        },
        {
          level: "Tertiary Education",
          institution: "Asia Pacific College",
        },
      ],
    };
  },
};
</script>

<style></style>