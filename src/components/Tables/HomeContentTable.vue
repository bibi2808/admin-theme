<template>
  <div>
    <md-table v-model="listPages" :table-header-color="tableHeaderColor">
      <md-table-row slot="md-table-row" slot-scope="{ item }">
        <md-table-cell md-label="Name" class="md-title">{{ item.title }}</md-table-cell>
        <md-table-cell md-label="Content">{{ item.content }}</md-table-cell>
      </md-table-row>
    </md-table>
  </div>
</template>

<script>
export default {
  name: "home-content-table",
  props: {
    tableHeaderColor: {
      type: String,
      default: ""
    }
  },
  data() {
    return {
      selected: [],
      listPages: [
        {
          title: "管理者ユーザー",
          content: "管理者の追加や、権限の管理ができます。マニュアルはこちら。"
        },
        {
          title: "外部リンク編集",
          content: "スレッド下のアイコン画像やリンク先の設定ができます。マニュアルはこちら。"
        },
        {
          title: "スレッド",
          content: "スレッド管理や配信機能、データ閲覧ができます。マニュアルはこちら。"
        },
        {
          title: "ユーザー管理",
          content: "ユーザー情報の閲覧、管理ができます。マニュアルはこちら。"
        },
        {
          title: "計測機能",
          content: "登録導線、一斉配信、ステップメールの計測結果を確認できます。マニュアルはこちら。",
        }
      ]
    };
  },
};
</script>
