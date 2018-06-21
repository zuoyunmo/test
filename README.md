<!DOCTYPE html> 
<html> 
<body> 
<h1>这是一个标题</h1>
<h2>这是一个标题</h2>
<h3>这是一个标题</h3>
<h1>Test</h1>
<hr style="height:5px;border:none;border-top:50px solid #2894ff;" />
<hr style=" height:2px;border:none;border-top:2px dotted #185598;" />
<h3>Test 1</h3>
<?php 
// echo "<div style='background:#ff0000; width:300px; height:300px;'>";
// echo 'Test 1';
// echo '<br>';
$x = "World!";
echo $x;
echo '<br>';
$s = 'Hello';
echo $s;
echo '<br>';
echo $s.' '.$x;
echo '<br>';
echo strlen('hello word!');
echo '<br>';
echo strpos("hello word!","o");
echo '<br>';
?>
<hr style=" height:2px;border:none;border-top:2px dotted #185598;" />
<h3>Test 2</h3>
<?php
// echo 'Test 2';
// echo '<br>';
$s = 9.6e6;
echo $s;
echo '<br>';
var_dump($s);
echo '<br>';
echo '<br>';
$im = imagecreatetruecolor(300,1000);
$red = imagecolorallocate($im,255,0,0);
imageline($im,30,30,240,140,$red);
imagepng($im);
imagedestroy($im);
?>
<hr style=" height:2px;border:none;border-top:2px dotted #185598;" />
<h3>Test 3</h3>
<?php
// echo 'Test 3';
// echo '<br>';
$x=5;
$y=3;
echo 'x='.$x;
echo '<br>';
echo 'y='.$y;
echo '<br>';
echo '<br>';
print 'z1='.$z=$x+$y;
echo '<br>';
echo 'z1='.$x+=$y;
echo '<br>';
echo '<br>';
echo '-(z1)='.$z=-$x;
echo '<br>';
echo '<br>';
print 'z2='.$z=$x*$y;
echo '<br>';
echo 'z2='.$x*=$y;
echo '<br>';
print 'z3='.$z=$x/$y;
echo '<br>';
echo 'z3='.$x/=$y;
echo '<br>';
print 'z4='.$z=$x%$y;
echo '<br>';
echo 'z4='.$x%=$y;
echo '<br>';
echo '<br>';
$x=7;
echo ++$x." //"."($x=7,echo ++$x)";
echo '<br>';
$y=10;
echo $y++."//"."(y=10,echo y++)";
echo '<br>';
echo $y."//"."(echo y)";
echo '<br>';
echo '<br>';
echo '<br>';
?>
<hr style=" height:2px;border:none;border-top:2px dotted #185598;" />
<h3>Test 4</h3>
<?php
// echo 'Test 4';
// echo '<br>';
class Car
{
    var $color;
    function __construct($color="green") {
        $this->color = $color;
    }
    function what_color(){
        return $this->color;
    }
}
function print_vars($obj) {
    foreach (get_object_vars($obj) as $prop => $val) {
        echo "\t$prop = $val\n";
    }
}
$herbie = new Car("white");
echo "\therbie: Properties\n";
print_vars($herbie);
echo '<br>';
echo '<br>';
$x="Hello world!";
$x=null;
var_dump($x);
echo '<br>';
echo '<br>';
?>
<hr style=" height:2px;border:none;border-top:2px dotted #185598;" />
<h3>Test 5</h3>
<?php
// echo 'Test 5';
// echo '<br>';
// define("GREETING", "欢迎访问 Runoob.com");
define("greeting", "欢迎访问 runoob.COM",true);
echo GREETING;
echo '<br>';
echo greeting;
echo '<br>';
?>
<hr style=" height:2px;border:none;border-top:2px dotted #185598;" />
<h3>Test 6</h3>
<?php
// echo 'Test 6';
// echo '<br>';
for ($i=1; $i<=10; $i++)
{
    if ($i % 2 == 1)
    {
        echo "<ins>" . $i . "</ins>".",";
    }
    elseif($i<10 ) 
    {
        echo $i.',';
    }
    else
    {
        echo $i."。"; 
    }
}
?>
<hr style=" height:2px;border:none;border-top:2px dotted #185598;" />
<h3>Test 7</h3>
<?php
// echo 'Test 7';
$x=7;
$y=10;
echo 'x='.$x;
echo '<br>';
echo 'y='.$y;
echo '<br>';
var_dump($x>10 and $y>5);
echo '<br>';
var_dump($x!=$y);
echo '<br>';
var_dump($x||$y);
echo '<br>';
echo '<br>';
$x=array("a"=>"red","b"=>"green","c"=>"white");
$y=array("d"=>"blue","e"=>"yellow","f"=>"black");
$z=$x+$y;
var_dump($z);
?> 
<hr style=" height:2px;border:none;border-top:2px dotted #185598;" />
</body> 
</html>