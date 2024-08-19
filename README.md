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

<h2>Global and Local Variabl</h2>
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

<h2>Fetch and display row from database Table</h2>
<code>
$servername = "localhost";
$username = "root";
$password = "";
$database = "dbname";

$conn = mysqli_connect($servername, $username, $password, $database);

$sql = "SELECT * FROM `table_name`";
$result = mysqli_query($conn, $sql);

// Find the number of records 
$num = mysqli_num_rows($result);
echo $num;
echo " records found in the DataBase<br>";

// Display the rows returned by the sql query
if($num> 0){
     $row = mysqli_fetch_assoc($result);
     echo var_dump($row);
     echo "<br>";

     $row = mysqli_fetch_assoc($result);
     echo var_dump($row);
     echo "<br>";
}  
</code>   
<h2>We can fetch in a better way using the while loop</h2>
<code>
if($num> 0){
     while($row = mysqli_fetch_assoc($result)){
        echo var_dump($row);
        echo $row['sno'] .  ". Hello ". $row['name'] ." Welcome to ". $row['dest'];
        echo "<br>";
    } 
}
</code>
<h2>Read any file</h2>
<code>
$a = readfile("myfile.txt");
echo $a;

readfile("myfile.txt");
readfile("1.png");
readfile("file.html");
</code>
