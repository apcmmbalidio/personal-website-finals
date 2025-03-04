<template>
  <card class="card" title="User Profile">
    <div>
      <div class="row">
        <div class="col-md-6">
          <div class="profile-info">
            <label>Course</label>
            <p>{{ user.Course }}</p>
          </div>
        </div>
        <div class="col-md-6">
          <div class="profile-info">
            <label>Nickname</label>
            <p>{{ user.Nickname }}</p>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-md-6">
          <div class="profile-info">
            <label>First Name</label>
            <p>{{ user.firstName }}</p>
          </div>
        </div>
        <div class="col-md-6">
          <div class="profile-info">
            <label>Last Name</label>
            <p>{{ user.lastName }}</p>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-md-12">
          <div class="profile-info">
            <label>Address</label>
            <p>{{ user.address }}</p>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-md-12">
          <div class="profile-info">
            <label>About Me</label>
            <p>{{ user.aboutMe }}</p>
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
      user: {
        Course: "Computer Science - Software Systems",
        Nickname: "P",
        firstName: "Maria Sophea",
        lastName: "Balidio",
        address: "Silang, Cavite",
        aboutMe: "I’m a huge fan of psychological thrillers, horror, and musicals — Cabaret is one of my all-time favorite films because it blends all three genres!.",
      },
    };
  },
};
</script>

<style>
.profile-info {
  padding: 15px;
  border: 1px solid #ddd;
  border-radius: 5px;
  margin-bottom: 10px;
  background-color: #f9f9f9;
}

label {
  font-weight: bold;
  display: block;
  margin-bottom: 5px;
}
</style>