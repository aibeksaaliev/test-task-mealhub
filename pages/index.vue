<template>
  <main>
    <table class="comments-table">
      <thead>
      <tr>
        <th class="column-id">ID</th>
        <th class="column-name">Name</th>
        <th class="column-email">Email</th>
        <th class="column-link">
          <div class="pagination-controllers">
            <button class="pagination-btn prev-btn">Prev</button>
            <span>1</span>
            <button class="pagination-btn next-btn">Next</button>
          </div>
        </th>
      </tr>
      </thead>
      <tbody>
      <tr>
        <td class="column-id">1</td>
        <td class="column-name">Aibek</td>
        <td class="column-email">dokaidea@gmail.com</td>
        <td class="column-link"><nuxt-link class="comment-link" to="comments/id">Link</nuxt-link></td>
      </tr>
      <tr>
        <td class="column-id">1</td>
        <td class="column-name">Aibek</td>
        <td class="column-email">dokaidea@gmail.com</td>
        <td class="column-link"><nuxt-link class="comment-link" to="comments/id">Link</nuxt-link></td>
      </tr>
      </tbody>
    </table>
  </main>
</template>

<script>
export default {
  name: 'Comments'
}
</script>

<style>
.comments-table {
  width: 100%;
  text-align: left;
  border-collapse: collapse;
  border-radius: 10px 10px 0 0;
  overflow: hidden;
}

.comments-table thead {
  background-color: #36304a;
  color: #FFFFFF;
  height: 60px;
}

.comments-table tbody {
  color: #808080;
  font-size: 15px;
}

.column-id {
  width: 100px;
  padding-left: 40px;
}

.column-name {
  width: 250px;
  padding-left: 10px;
}

.column-email {
  width: 250px;
  padding-left: 10px;
}

.column-link {
  width: 100px;
  padding-left: 10px;
  text-align: center;
}

.comments-table tbody tr {
  height: 50px;
}

.comments-table tbody tr:hover {
  background-color: #F5F5F5;
  color: #303030;
}

.comments-table tbody tr:nth-child(even) {
  background-color: #F5F5F5;
}

.pagination-btn {
  width: 20px;
  height: 20px;
  overflow: hidden;
  text-indent: -50px;
  border-radius: 50%;
  border: none;
  background-image: url("static/arrow-ic.svg");
  background-color: #FFFFFF;
  background-position: center;
  background-repeat: no-repeat;
}

.pagination-btn:hover {
  box-shadow: 0 0 3px 1px rgba(255,255,255,0.75);
}

.pagination-btn:active {
  box-shadow: 0 0 3px 1px rgba(0,0,0,0.75);
}

.prev-btn {
  transform: rotate(180deg);
}

.comment-link {
  text-decoration: none;
  display: inline-block;
  width: 25px;
  height: 25px;
  border-radius: 50%;
  overflow: hidden;
  text-indent: -60px;
  background-image: url("static/arrow-ic-white.svg");
  background-color: #36304a;
  background-position: center;
  background-repeat: no-repeat;
}

.comment-link:hover {
  box-shadow: 0 0 3px 1px rgba(0,0,0,0.75);
}

</style>
