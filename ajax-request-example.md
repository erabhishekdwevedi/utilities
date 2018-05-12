
# Ajax Request Example. 
* Using ajax() method to get json response

```

<!DOCTYPE html>
<html>
<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>

<script>

	$(document).ready(function(){

			$.ajax({
					url: "https://jsonplaceholder.typicode.com/comments",
				//	type: 'POST',
				//  data: data,
				
					beforeSend: function(){ $("#message").append("<li> Before Send </li>");},  	
					error:      function (xhr,status,error){ $("#message").append("<li> Error </li>");},
				    complete:   function(xhr,status) { $("#message").append("<li> Complete </li>");},
				    success:    function(xhr,status,error){ $("#message").append("<li> Success </li>"); }
				
				  });	
	});  
</script>
</head>
<body>

<div id="message"><h2>AJAX Flow </h2></div>

</body>
</html>
```
