<template>
  <div class="main">
    <div class="container-body">
      <div class="employee">
        <h2 class="name">Employee</h2>
        <button class="add" data-toggle="modal" data-target="#exampleModal">Add New</button>
      </div>
      <!-- <div
        class="modal fade"
        id="exampleModal"
        tabindex="-1"
        role="dialog"
        aria-labelledby="exampleModalLabel"
        aria-hidden="true"
      >
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <div class="modal-header">
              <h5 class="modal-title" id="exampleModalLabel">Modal title</h5>
              <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                <span aria-hidden="true">&times;</span>
              </button>
            </div>
            <div class="modal-body">
              ...
            </div>
            <div class="modal-footer">
              <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
              <button type="button" class="btn btn-primary">Save changes</button>
            </div>
          </div>
        </div>
      </div> -->
      <div class="employee details">
        <h4 class="name">Josh Bakery Ventures</h4>
        <div class="address">
          <h5 class="name">62, Bode Thomas, Surulere, Lagos</h5>
        </div>
      </div>
      <div class="filters">
        <div class="search"></div>
        <div class="pagination"></div>
      </div>
      <div class="table-surround">
        <div class="table">
          <div class="table-head">
            <div>
              <div class="checkbox"></div>
            </div>
            <div>
              <p>FIRST NAME</p>
            </div>
            <div>
              <p>LAST NAME</p>
            </div>
            <div>
              <p>EMAIL</p>
            </div>
            <div>
              <p>PHONE</p>
            </div>
            <div>
              <p>ROLE</p>
            </div>
            <div></div>
          </div>
          <div class="table-row" v-for="i in 10" :key="i">
            <div>
              <div class="checkbox"></div>
            </div>
            <div>
              <p>Joshua</p>
            </div>
            <div>
              <p>Bakare</p>
            </div>
            <div>
              <p>jognbakery@gmail.com</p>
            </div>
            <div>
              <p>+2348123444803</p>
            </div>
            <div>
              <p>Staff</p>
            </div>
            <div>
              <p @click="deleteEmployee(employee.id)">
                <svg xmlns="http://www.w3.org/2000/svg" width="18" height="21" viewBox="0 0 18 21" fill="none">
                  <path
                    d="M1 5.55555H2.77778H17"
                    stroke="#6A7E8A"
                    stroke-width="1.2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M3.9778 5.55555C3.9778 4.89281 3.44054 4.35555 2.7778 4.35555V5.55555H3.9778ZM3.9778 18V5.55555H2.7778V18H3.9778ZM4.55557 18.5778C4.23647 18.5778 3.9778 18.3191 3.9778 18H2.7778C2.7778 18.9818 3.57373 19.7778 4.55557 19.7778V18.5778ZM13.4445 18.5778H4.55557V19.7778H13.4445V18.5778ZM14.0222 18C14.0222 18.3191 13.7636 18.5778 13.4445 18.5778V19.7778C14.4263 19.7778 15.2222 18.9818 15.2222 18H14.0222ZM14.0222 5.55555V18H15.2222V5.55555H14.0222ZM15.2222 4.35555C14.5595 4.35555 14.0222 4.89281 14.0222 5.55555H15.2222H15.2222V4.35555ZM16.4222 5.55555C16.4222 4.89281 15.885 4.35555 15.2222 4.35555V5.55555H16.4222ZM16.4222 18V5.55555H15.2222V18H16.4222ZM13.4445 20.9778C15.089 20.9778 16.4222 19.6446 16.4222 18H15.2222C15.2222 18.9818 14.4263 19.7778 13.4445 19.7778V20.9778ZM4.55557 20.9778H13.4445V19.7778H4.55557V20.9778ZM1.5778 18C1.5778 19.6446 2.91099 20.9778 4.55557 20.9778V19.7778C3.57373 19.7778 2.7778 18.9818 2.7778 18H1.5778ZM1.5778 5.55555V18H2.7778V5.55555H1.5778ZM2.7778 4.35555C2.11505 4.35555 1.5778 4.89281 1.5778 5.55555H2.7778V4.35555ZM6.64446 3.77777C6.64446 3.45867 6.90314 3.19999 7.22224 3.19999V1.99999C6.2404 1.99999 5.44446 2.79593 5.44446 3.77777H6.64446ZM6.64446 5.55555V3.77777H5.44446V5.55555H6.64446ZM5.44446 6.75555C6.1072 6.75555 6.64446 6.21829 6.64446 5.55555H5.44446V6.75555ZM4.24446 5.55555C4.24446 6.21829 4.78172 6.75555 5.44446 6.75555V5.55555H4.24446ZM4.24446 3.77777V5.55555H5.44446V3.77777H4.24446ZM7.22224 0.799994C5.57766 0.799994 4.24446 2.13319 4.24446 3.77777H5.44446C5.44446 2.79593 6.2404 1.99999 7.22224 1.99999V0.799994ZM10.7778 0.799994H7.22224V1.99999H10.7778V0.799994ZM13.7556 3.77777C13.7556 2.13319 12.4224 0.799994 10.7778 0.799994V1.99999C11.7596 1.99999 12.5556 2.79593 12.5556 3.77777H13.7556ZM13.7556 5.55555V3.77777H12.5556V5.55555H13.7556ZM12.5556 6.75555C13.2183 6.75555 13.7556 6.21829 13.7556 5.55555H12.5556V6.75555ZM11.3556 5.55555C11.3556 6.21829 11.8928 6.75555 12.5556 6.75555V5.55555H11.3556ZM11.3556 3.77777V5.55555H12.5556V3.77777H11.3556ZM10.7778 3.19999C11.0969 3.19999 11.3556 3.45867 11.3556 3.77777H12.5556C12.5556 2.79593 11.7596 1.99999 10.7778 1.99999V3.19999ZM7.22224 3.19999H10.7778V1.99999H7.22224V3.19999Z"
                    fill="#6A7E8A"
                  />
                  <path
                    d="M7.22222 9.99999V15.3333"
                    stroke="#6A7E8A"
                    stroke-width="1.2"
                    stroke-linecap="square"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M10.7778 9.99999V15.3333"
                    stroke="#6A7E8A"
                    stroke-width="1.2"
                    stroke-linecap="square"
                    stroke-linejoin="round"
                  />
                </svg>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import axios from "axios";
export default {
  data() {
    return {
      employee: {
        first_name: "Busayo",
        last_name: "Dawodu",
        email: "johndoe@yahoo.com",
        phone: "08123444894",
        role: "Staff",
      },
      employee: [],
    };
  },
  mounted() {
    this.addEmployee();
  },
  methods: {
    addEmployee() {
      //   console.log("hi");
      this.$http
        .post(`https://crudcrud.com/api/d404675c998a47a481c3e270447933cc`, this.employee)
        .then((response) => {
          console.log(response);
        })
        .catch((e) => {
          console.log(e);
        });
    },
    deleteEmployee(id) {
      this.$http
        .delete(`https://crudcrud.com/api/d404675c998a47a481c3e270447933cc/${id}`)
        .then((response) => {
          console.log(response);
        })
        .catch((e) => {
          console.log(e);
        });
    },
    getEmployee() {
      this.$http
        .get(`https://crudcrud.com/api/d404675c998a47a481c3e270447933cc`)
        .then((response) => {
          console.log(response);
        })
        .catch((e) => {
          console.log(e);
        });
    },
    editEmployee(id) {
      this.$http
        .put(`https://crudcrud.com/api/d404675c998a47a481c3e270447933cc/${id}`, this.employee)
        .then((response) => {
          console.log(response);
        })
        .catch((e) => {
          console.log(e);
        });
    },
  },
};
</script>
<style scoped>
.main {
  background-color: #f6f8f8;
  height: 100%;
}
.container-body {
  width: 90%;
  margin: auto;
}
.employee {
  display: flex;
  justify-content: space-between;
  align-items: center;
  /* padding: 1rem; */
  width: 100%;
}
.name {
  color: var(--primary-color);
}
.add {
  background-color: var(--green);
  color: white;
  padding: 0.5rem 2rem;
  border-radius: 3px;
  border: none;
}
.details {
  background-color: white;
  border-radius: 5px;
  padding: 2rem 1rem;
}
.table-row,
.table-head {
  display: grid;
  grid-template-columns: repeat(7, 14.28%);
  margin-top: 1em;
  align-items: center;
  /* justify-items: center; */
}
.table {
  overflow-x: auto;
}
.checkbox {
  border-radius: 5px;
  height: 1rem;
  width: 1rem;
  background-color: white;
  border: 1px solid rgba(106, 126, 138, 0.4);
  margin: auto;
}
.table-row {
  background-color: white;
  border-radius: 5px;
  margin: 1rem 0;
}
.table-head div > p,
.table-row div > p {
  color: var(--primary-color);
}
@media only screen and (max-width: 768px) {
  .table-row,
  .table-head {
    grid-template-columns: repeat(7, auto);
    grid-template-rows: 100%;
    /* overflow-y: auto; */
    grid-column-gap: 0.5rem;
    padding: 0 0.5rem;
  }
  /* .table-row {
    width: auto;
  } */
  .details {
    padding: 0rem 0.5rem;
  }
  .table {
    width: 40rem;
  }
  .container-body {
    overflow-y: auto;
  }
  .table-surround {
    overflow-y: auto;
  }
  .table-head div > p {
    font-size: 1rem;
  }
}
</style>
