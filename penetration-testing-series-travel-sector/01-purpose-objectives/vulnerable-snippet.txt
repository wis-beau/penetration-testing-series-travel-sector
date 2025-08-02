// UNSAFE EXAMPLE
$promo = $_GET['code'];
$query = "SELECT * FROM bookings WHERE promo_code = '$promo'";
$result = mysqli_query($conn, $query);
