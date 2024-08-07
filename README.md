# PHP_command

<h2>Connect to database:</h2>
<code>
$servername = "localhost";
$username = "root";
$password = "";
$dbname = "crud_example";
// Create connection
$conn = new mysqli($servername, $username, $password, $dbname);
</code>

<h2>Connect to database:</h2>
<code>
<?php
   $con= mysqli_connect('localhost','root');
   if($con){
       echo "Connection Successful";
   }
   else{
       echo "Connection Failed";
   }

   mysqli_select_db($con,'photography');

   $name= $_POST['name'];
   $emai= $_POST['email'];
   $number= $_POST['number'];

   $query= "INSERT INTO users(name,email,number) VALUES('$name','$emai','$number')";

   mysqli_query($con,$query);
   header('location:index.php');
?>
</code>

<h2>Function for sum of array</h2>
<code>
function sumofarr($marksArr){
    $sum=0;
    foreach($variable as $value){
        $sum+= $value;
    }
    return $sum;
}
$me = [34,56,67,87];
$sumofmark= sumofarr($me);
</code>