<template>
  <div class="main">
    <h1 class="greeting">Hello Evano 👋🏼,</h1>
    <div class="customers">
      <div class="customers__head">
        <div class="customers__info">
          <h5 class="customers__info__title">All Customers</h5>
          <h5 class="customers__info__subtitle">Active Members</h5>
        </div>
        <div class="customers__search">
          <input  type="text" name="search" placeholder="Search">
        </div>
      </div>
      <div class="table-container">
        <table class="customers__table">
          <thead>
          <tr>
            <th>Customer Name</th>
            <th>Company</th>
            <th>Phone Number</th>
            <th>Email</th>
            <th>Country</th>
            <th>Status</th>
          </tr>
          </thead>
          <tbody>
          <tr v-for="customer in customers" :key="customer.email">
            <td class="customers__table__col customers__table__coll--name">{{ customer.name }}</td>
            <td class="customers__table__col customers__table__coll--company">{{ customer.company }}</td>
            <td class="customers__table__col customers__table__coll--phone">{{ customer.phoneNumber }}</td>
            <td class="customers__table__col customers__table__coll--email">{{ customer.email }}</td>
            <td class="customers__table__col customers__table__coll--country">{{ customer.country }}</td>
            <td class="customers__table__col customers__table__coll--status" :class="customer.status.toLowerCase()">
              <span>{{ customer.status }}</span>
            </td>
          </tr>
          </tbody>
        </table>
      </div>
      <div class="customers__footer">
        <div class="customers__footer__data">
          Showing data 1 to 8 of  256K entries
        </div>
        <div class="customers__pagination">
          <button class="customers__pagination__btn"><</button>
          <button class="customers__pagination__btn customers__pagination__btn--active">1</button>
          <button class="customers__pagination__btn">2</button>
          <button class="customers__pagination__btn">3</button>
          <button class="customers__pagination__btn">4</button>
          <div class="customers__pagination__dots">...</div>
          <button class="customers__pagination__btn">40</button>
          <button class="customers__pagination__btn">></button>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  data() {
    return {
      customers: [
        {
          "name": "John Doe",
          "company": "ABC Corp",
          "phoneNumber": "123-456-7890",
          "email": "john.doe@example.com",
          "country": "USA",
          "status": "Active"
        },
        {
          "name": "Alice Johnson",
          "company": "XYZ Ltd",
          "phoneNumber": "987-654-3210",
          "email": "alice.johnson@example.com",
          "country": "Canada",
          "status": "Inactive"
        },
        {
          "name": "Bob Smith",
          "company": "123 Industries",
          "phoneNumber": "555-123-4567",
          "email": "bob.smith@example.com",
          "country": "UK",
          "status": "Active"
        },
        {
          "name": "Eva Miller",
          "company": "Sunshine Corp",
          "phoneNumber": "111-222-3333",
          "email": "eva.miller@example.com",
          "country": "Australia",
          "status": "Active"
        },
        {
          "name": "David White",
          "company": "Tech Innovations",
          "phoneNumber": "444-555-6666",
          "email": "david.white@example.com",
          "country": "Germany",
          "status": "Inactive"
        },
        {
          "name": "Sophia Davis",
          "company": "Global Solutions",
          "phoneNumber": "777-888-9999",
          "email": "sophia.davis@example.com",
          "country": "France",
          "status": "Active"
        },
        {
          "name": "Matthew Brown",
          "company": "Future Tech",
          "phoneNumber": "123-456-7890",
          "email": "matthew.brown@example.com",
          "country": "USA",
          "status": "Active"
        },
        {
          "name": "Olivia Wilson",
          "company": "Innovate Co",
          "phoneNumber": "987-654-3210",
          "email": "olivia.wilson@example.com",
          "country": "Canada",
          "status": "Inactive"
        }
      ]
    };
  }
};
</script>