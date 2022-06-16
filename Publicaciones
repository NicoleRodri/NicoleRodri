<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Document</title>
	<link rel="stylesheet" type="text/css" href="bootstrap.min.css">
	<script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4=" crossorigin="anonymous"></script>
	<script>
   $(document).on("click","#btn_publicar",()=>{
   	
   	const user=$("pub_usuario").val();
   	const desc=$("pub_descripcion").val();
   	const estado=$("pub_estado").val();

   	$.ajax({
   		url:'accionespublicaciones.php',
   		data:{user:user,desc:desc,estado},
   		type:'POST',
   		dataType:'json',
   		succes:(data)=>{
   			console.log(data);
   		},
   		$("#estado").text(data[0].pub_estado);
   		$("#publicacion").text(data[0].pub_descripcion);
   		if(data)[0].pub_estado=='alegre'{
        $("cont _publicacion").removeClass("bg_succes");
        $("cont _publicacion").removeClass("bg_warning");
        $("cont _publicacion").addClass("bg_succes");

        if(data)[0].pub_estado=='triste'{
        $("cont _publicacion").removeClass("bg_succes");
        $("cont _publicacion").removeClass("bg_warning");
        $("cont _publicacion").addClass("bg_succes");

        if(data)[0].pub_estado=='molesto	'{
        $("cont _publicacion").removeClass("bg_succes");
        $("cont _publicacion").addClass("bg_warning");
        $("cont _publicacion").addClass("bg_succes");




   		}
   		error:(desc,estado)=>{},

   		
   	})

   });
   </script>
<body>

	<h1 class="bg-success">VN-Book</h1>
	<div class="container">

		<div class="row">
			<div class="col-md-6">
			<input type="text" id="pub_usuario" placeholder="usuario" class="form-control">
		<textarea name="id" class="form-control bg-dark"></textarea> 
		

		<select name="" id="" class="form-control bg-dark">
		<option value="">Elige una opcion</option>
		<option value="alegre">alegre</option>
	    <option value="triste">triste</option>
	    	<option value="molesto">molesto</option>
	    	</select>

	    	<div class="d-grid-gap-2">
	    	<button class="btn btn-primary">Publicar</button>
	    	</div>
	</div>
	</div>
		</div> 
		    <div class="card_cont publicacion"></div>
			<div class="col-md-6">Foto</div>
			<img src="no image available_files" width="30px" aly>
			<div class="card-body">

				<h1 class=" estado">Estado</h1>
				<P class="card-text" id="publicacion">Descripcion</P>
			</div> 
		
		
</body>
</html>

<!---
NicoleRodri/NicoleRodri is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
