<script>
const axios = require("axios");
async function some() {const result = await axios
.get('http://localhost:4747/user')
.then((response)=>{
    console.log(response.data)
    return response.data;
}).catch((err)=>console.log(err));}
some();
</script>