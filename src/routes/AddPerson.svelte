<script>    
let name
let age
let city

const AddPerson=()=>{
    console.log(name,age,city);
}
</script>

<form action="" on:submit|preventDefault={AddPerson}>
    Name: <input type="text" name="name" id="" bind:value={name}/><br/>
    Age:<input type="text" name="age" id="" bind:value={age}/><br/>
    City:   <input type="text" name="name" id="" bind:value={city}/><br/>
        <button>Submit</button>
</form>