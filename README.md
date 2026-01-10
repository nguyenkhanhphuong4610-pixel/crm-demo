# spa-demo
Web demo quản lý khách hàng spa
<button onclick="addCustomer()">Thêm khách</button>
<script>
let customers = [];

function addCustomer() {
  const name = document.getElementById("name").value;
  const phone = document.getElementById("phone").value;
  const service = document.getElementById("service").value;
  const date = document.getElementById("date").value;

  if (!name || !phone || !service || !date) {
    alert("Vui lòng nhập đủ thông tin");
    return;
  }

  customers.push({ name, phone, service, date });
  render();
}
</script>
