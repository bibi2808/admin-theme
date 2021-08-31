<template>
  <!-- <div class="content">
    <div class="md-layout">
      <div class="md-layout-item md-medium-size-100 md-size-66">
        <edit-profile-form data-background-color="green"> </edit-profile-form>
      </div>
      <div class="md-layout-item md-medium-size-100 md-size-33">
        <user-card> </user-card>
      </div>
    </div>
  </div> -->
  <div class="content">
    <div class="md-layout">
      <div
        class="md-layout-item md-medium-size-100 md-xsmall-size-100 md-size-100"
      >
        <md-card>
          <md-card-header data-background-color="green">
            <h4 class="title">管理者ユーザー一覧</h4>
            <md-button class="md-primary">新規追加</md-button>
            <!-- <p class="category">Here is a subtitle for this table</p> -->
          </md-card-header>
          <md-card-content>
            <AdminListTable table-header-color="green" ></AdminListTable>
          </md-card-content>
        </md-card>
      </div>
    </div>
  </div>
</template>

<script>
import AdminListTable from "../components/Tables/AdminListTable.vue";
// import { EditProfileForm, UserCard } from "@/pages";

export default {
  components: {
    AdminListTable
    // EditProfileForm,
    // UserCard
  }
};
</script>
