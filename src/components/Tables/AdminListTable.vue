<template>
  <div>
    <md-table v-model="listPages" :table-header-color="tableHeaderColor">
      <md-table-row slot="md-table-row" slot-scope="{ item }">
        <md-checkbox v-model="array" value="1">Array</md-checkbox>
        <md-table-cell md-label="ID">{{ item.id }}</md-table-cell>
        <md-table-cell md-label="権限">{{ item.role }}</md-table-cell>
      </md-table-row>
    </md-table>
  </div>
</template>

<script>
export default {
  name: "admin-list-table",
  props: {
    tableHeaderColor: {
      type: String,
      default: "",
    },
  },
  data() {
    return {
        array: [],
      listPages: [
        {
          id: "cross123@cross-staff.com",
          role: "マスター",
          value:1
        },
        {
          id: "cross456@cross-staff.com",
          role: "ディレクター",
          value:4
        },
        {
          id: "cross789@cross-staff.com",
          role: "サポート",
          value:3
        },
        {
          id: "crossJQK@cross-staff.com",
          role: "閲覧",
          value:2
        },
        {
          id: "cross999@cross-staff.com",
          role: "マスター",
          value:5
        },
        {
          id: "cross888@cross-staff.com",
          role: "ディレクター",
          value:6
        },
        {
          id: "cross777@cross-staff.com",
          role: "サポート",
          value:7
        },
        {
          id: "cross666@cross-staff.com",
          role: "閲覧",
          value:8
        },
      ],
    };
  },
};
</script>

<style>
</style>