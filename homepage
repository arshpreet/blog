<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<!--
Design by TEMPLATED
http://templated.co
Released for free under the Creative Commons Attribution License

Name       : TwoFold 
Description: A two-column, fixed-width design with dark color scheme.
Version    : 1.0
Released   : 20130526

-->
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title></title>
<meta name="keywords" content="" />
<meta name="description" content="" />
<link href="http://fonts.googleapis.com/css?family=Open+Sans:300,600,700" rel="stylesheet" />
<link href="default.css" rel="stylesheet" type="text/css" media="all" />
<!--[if IE 6]>
<link href="default_ie6.css" rel="stylesheet" type="text/css" />
<![endif]-->
</head>
<body>
<form action="check_sign.php" method="POST">
<div id="header" class="container">
	<div id="logo">
		<h1><a>bloghub</a></h1>
	</div>
	<div id="menu">
		<ul>
			
			<li><input type="text" name="username" placeholder="Username"></li>
			<li><input type="password" name="password" placeholder="Password"></li>
			<li><input type="submit" class="login-submit" name="login" value="LOGIN"></li>
			
			<li><a href="http://localhost/blogger/register.php" accesskey="2" title="">REGISTER</a></li>
			<li><a href="#" accesskey="3" title="">ABOUT US</a></li>
			
		</ul>
	</div>
</div>
<div id="wrapper">
	
	<div id="page" class="container">
		<div id="content">
			<div class="title">
				<h2>latest blogs</h2>
				
		</div>
		<?php
			$servername = "localhost";
			$username = "root";
			$password = "";
			$dbname = "blog";

			// Create connection
			$conn = mysqli_connect($servername, $username, $password,$dbname);
			// Check connection
			if (!$conn) {
				die("Connection failed: " . mysqli_connect_error());
			}
		
				$sql="SELECT * FROM post WHERE permission='1' ORDER BY postid DESC";
				$result=mysqli_query($conn,$sql);
   
    while($row = mysqli_fetch_assoc($result)) {
       
		
    
 
				?>

			<h3><?php echo $row['title']; ?></h3>
			posted by <a href="http://localhost/blogger/blogger.php?username=<?php echo $row['username']; ?>"><?php echo $row['username']; ?></a> on <?php echo $row['date'];?><br/>
			<h3><?php echo $row['post'];?></h3>
			<?php } ?>
	</div>
</div>
<div id="featured-wrapper">
	<div id="featured" class="container">
		<div id="box1">
			<div>
			<h2>BLOGS</h2>
			</div>
			<?php
			$servername = "localhost";
			$username = "root";
			$password = "";
			$dbname = "blog";

			// Create connection
			$conn = mysqli_connect($servername, $username, $password,$dbname);
			// Check connection
			if (!$conn) {
				die("Connection failed: " . mysqli_connect_error());
			}
			$sql = "SELECT DISTINCT title FROM post WHERE permission='1'";
			$result=mysqli_query($conn,$sql);
			while($row = mysqli_fetch_assoc($result)) {
				?>
				
				
			<ul class="style1">
				<li class="first"><a href="#"><?php echo $row['title']; ?></a></li>
			</ul>
			<?php } ?>
		</div>
		<div id="box2">
			<div>
				<h2>USERS</h2>
			</div>
			<?php
			$servername = "localhost";
			$username = "root";
			$password = "";
			$dbname = "blog";

			// Create connection
			$conn = mysqli_connect($servername, $username, $password,$dbname);
			// Check connection
			if (!$conn) {
				die("Connection failed: " . mysqli_connect_error());
			}
			$sql = "SELECT DISTINCT username FROM blogger WHERE username!='admin' ";
			$result=mysqli_query($conn,$sql);
			while($row = mysqli_fetch_assoc($result)) {
				?>
			<ul class="style1">
				<li class="first"><a href="http://localhost/blogger/blogger.php?username=<?php echo $row['username']; ?>"><?php echo $row['username']; ?></a></li>
			</ul>
				<?php } ?>
		</div>
		
	</div>
</div>
<div id="footer" class="container">
	<div>
		<div>
			<h2>Get in touch</h2>
			<span class="byline">Phasellus nec erat sit amet nibh pellentesque congue</span> </div>
		<ul class="contact">
			<li><a href="#" class="icon icon-twitter"><span>Twitter</span></a></li>
			<li><a href="#" class="icon icon-facebook"><span></span></a></li>
			<li><a href="#" class="icon icon-dribbble"><span>Pinterest</span></a></li>
			<li><a href="#" class="icon icon-tumblr"><span>Google+</span></a></li>
			<li><a href="#" class="icon icon-rss"><span>Pinterest</span></a></li>
		</ul>
	</div>
	<p>&copy; Untitled. | Design by <a href="http://templated.co" rel="nofollow">ARSHPREET</a>.</p>
</div>
</body>
</html>
