# PHP_command

<h2>Connect to database:</h2>
<code>
$servername = "localhost";
$username = "root";
$password = "";
$dbname = "crud_example";
// Create connection
$conn = mysqli_connect($servername, $username, $password, $dbname);
if($conn){
       echo "Connection Successful";
   }
   else{
       echo "Connection Failed";
   }
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

<h2>Globaland Local Variabl</h2>
<code>
$a = 98; // Global Variabl
function printValue(){
    $a = 97; // Local Variable  
}
</code>

<h2>Create a Database</h2>
<code>
$sql = "CREATE DATABASE mydbase";
mysqli_query($conn, $sqli);
</code>