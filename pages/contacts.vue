<template>
  <main>
      <h1>Contacts</h1>
      <table>
          <thead>
              <th>#</th>
              <th>Firstname</th>
              <th>Lastname</th>
              <th>D.O.B.</th>
          </thead>
          <tbody>
              <tr v-for="contact in contacts" v-bind:key="contact.id">
                  <td>{{ contact.id }}</td>
                  <td>{{ contact.firstname }}</td>
                  <td>{{ contact.lastname }}</td>
                  <td>{{ contact.dob }}</td>
              </tr>
          </tbody>
      </table>
  </main>
</template>

<script>
export default {
  layout: 'loggedIn',
  data(){
      return {
          contacts: [
              {
                  id: '1',
                  firstname: 'Jane',
                  lastname: 'Doe',
                  dob: '04.07.1982'
              },
              {
                  id: '2',
                  firstname: 'John',
                  lastname: 'Doe',
                  dob: '28.04.1984'
              }
          ]
      }
  }
}
</script>

<style lang="sass">
main
    padding: 1rem 3rem

h1
    margin-top: 0

table, table th, table td
    border: 1px solid #333
    border-spacing: 0

table th, table td
    padding: 5px
    text-align: left

</style>