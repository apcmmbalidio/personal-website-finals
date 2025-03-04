<template>
  <card class="card full-height" title="Education List">
    <div class="education-container">
      <div class="row" v-for="education in educationList" :key="education.level">
        <div class="col-md-12">
          <div class="profile-info">
            <label>{{ education.level }}</label>
            <p>{{ education.institution }}</p>
          </div>
        </div>
      </div>
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

<style>
.full-height {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.education-container {
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.profile-info {
  padding: 20px;
  border: 1px solid #ddd;
  border-radius: 5px;
  margin-bottom: 10px;
  background-color: #f9f9f9;
  width: 100%;
}

label {
  font-weight: bold;
  display: block;
  margin-bottom: 5px;
}
</style>