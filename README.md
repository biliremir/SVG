<script>
document.addEventListener('DOMContentLoaded', function () {
  document.querySelectorAll('[data-bs-toggle="tooltip"]').forEach(el => {
    new bootstrap.Tooltip(el, {
      trigger: 'hover focus', // dokunmatik için focus da iyi
      delay: { "show": 100, "hide": 50 }
    });
  });
});
</script>
