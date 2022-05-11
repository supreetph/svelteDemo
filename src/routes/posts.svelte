<script context="module">   
export async function load({fetch}){
 let response=await fetch("https://jsonplaceholder.typicode.com/posts")
 const posts=await response.json()

 if (response.ok){
     return{
     props:{
         posts
     }
 }
}
}

</script>

<script>
    export let posts
</script>

<div>   
    <ul>
        {#each posts as post }
      <li>{post.title}</li>  
        {/each}
            
       
    </ul>
</div>