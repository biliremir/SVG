
<style>
.info-box {
  position: relative;
  display: inline-block;
}

.info-popup {
  display: none;
  position: absolute;
  top: 0;
  left: 120%; /* ikonun sağına */
  background: #fff;
  border: 1px solid #ccc;
  padding: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.2);
  z-index: 10;
}

.info-box:hover .info-popup {
  display: block;
}
</style>

<div class="info-box">
  <i class="bi bi-info-circle"></i>
  <div class="info-popup">
    <table border="1" cellpadding="4" cellspacing="0">
      <tr><th>Başlık</th><th>Değer</th></tr>
      <tr><td>A</td><td>10</td></tr>
      <tr><td>B</td><td>20</td></tr>
    </table>
  </div>
</div>
