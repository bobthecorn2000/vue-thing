<template>



	<div class="container">
		<h1 class="specialh1">Register Now</h1>
		<p>Please fill out the form below to register for classes at the Honorable Douglas Academy.</p>
		<form>
			<label for="name">Name:</label>
			<input type="text" id="name" name="name" required>

			<label for="email">Email:</label>
			<input type="email" id="email" name="email" required>

			<label for="password">Password:</label>
			<input type="password" id="password" name="password" required>

			<label for="confirm_password">Confirm Password:</label>
			<input type="password" id="confirm_password" name="confirm_password" required>

			<label for="grade">Grade Level:</label>
			<select id="grade" name="grade" required>
				<option value="">Select your grade level</option>
				<option value="9">9th grade</option>
				<option value="10">10th grade</option>
				<option value="11">11th grade</option>
				<option value="12">12th grade</option>
			</select>

			<div>

  
  <h3>Electives:</h3>
  <ul class="class-list">
    <li  class="class-item"><input type="checkbox" id="class-clowns-club" name="classes[]" value="Class Clowns Club"><label for="class-clowns-club">Class Clowns Club</label></li>
    <li  class="class-item"><input type="checkbox" id="calculus-club" name="classes[]" value="Calculus Club"><label for="calculus-club">Calculus Club</label></li>
    <li class="class-item"><input type="checkbox" id="culinary-class" name="classes[]" value="Culinary Class"><label for="culinary-class">Culinary Class</label></li>
    <li class="class-item"><input type="checkbox" id="computer-lab" name="classes[]" value="Computer Lab"><label for="computer-lab">Computer Lab</label></li>
    <li class="class-item"><input type="checkbox" id="art-class" name="classes[]" value="Art Class"><label for="art-class">Art Class</label></li>
    <li class="class-item"><input type="checkbox" id="photography" name="classes[]" value="Photography"><label for="photography">Photography</label></li>
    <li class="class-item"><input type="checkbox" id="orchestra" name="classes[]" value="Orchestra"><label for="orchestra">Orchestra</label></li>
    <li class="class-item"><input type="checkbox" id="arcade" name="classes[]" value="Arcade"><label for="arcade">Arcade</label></li>
    <li class="class-item"><input type="checkbox" id="media-studies" name="classes[]" value="Media Studies"><label for="media-studies">Media Studies</label></li>
    <li class="class-item"><input type="checkbox" id="physical-education" name="classes[]" value="Physical Education"><label for="physical-education">Physical Education</label></li>
    <li class="class-item"><input type="checkbox" id="class-pets" name="classes[]" value="Class Pets"><label for="class-pets">Class Pets</label></li>
    <li class="class-item"><input type="checkbox" id="robotics-club" name="classes[]" value="Robotics Club"><label for="robotics-club">Robotics Club</label></li>
  </ul>
</div>


			<button type="submit">Submit</button>
		</form>
	</div>


</template>
<style>

    button[type="submit"] {
  background-color: orange;
  
  border: none;
  border-radius: 4px;
  padding: 10px 20px;
  font-size: 18px;
  cursor: pointer;
  transition: all 0.3s ease;
}

button[type="submit"]:hover {
  background-color: black;
  color: orange;
}
.class-list {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

/* Style for each list item */
.class-item {
  margin: 10px 0;
}

/* Style for the checkbox */
.class-item input[type="checkbox"] {
  margin-right: 10px;
    
}

/* Style for the label text */
.class-item label {
  font-size: 18px;
  font-weight: bold;
  
}

.container {
  width: 75%;
  margin: 0 auto;
  background-color: #1f1f1f;
  padding: 30px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0,0,0,0.2);
}

.specialh1 {
  text-align: center;
  font-size: 32px;
  color: #FFA500;
}

input[type=text], input[type=email], input[type=password], select {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: none;
  border-radius: 4px;
}

input[type=submit] {
  background-color: #FFA500;
  color: #FFF;
  font-size: 16px;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  float: right;
}

input[type=submit]:hover {
  background-color: #FF8C00;
}

.row:after {
  content: "";
  display: table;
  clear: both;
}

.col-25 {
  float: left;
  width: 25%;
  margin-top: 6px;
}

.col-75 {
  float: left;
  width: 75%;
  margin-top: 6px;
}

@media screen and (max-width: 600px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 0;
  }
}
</style>