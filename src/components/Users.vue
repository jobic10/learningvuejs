<template>
    <div class="child">
    <table border="1">
<tr>
<th>ID</th>
<th>Name</th>
<th>Email</th>
</tr>
<tr v-for="user in users" :key="user.email">
<td>{{ user.id }}</td>
<td>{{ user.name }}</td>
<td>{{ user.email }}</td>
</tr>
</table>   
    </div>
</template>
<script>
export default {
    name: 'Users',
    props:{
        data:String
    },
    methods: {
        toggleDisplay(){
            this.show = !this.show
        }
    },
    data(){
        return{
            show:false,
            users:[
                {id:1,name:"Owonubi Job",email:'jobowonubi@gmail.com'},
                {id:2,name:"Ibrahim Faruq",email:'faruk@gmail.com'},
                {id:3,name:"Akinola Roseline",email:'rose@gmail.com'},
                {id:4,name:"Owonubi Solomon",email:'owonubi@gmail.com'},
                {id:5,name:"Akinola Peter",email:'akinola@gmail.com'},
                ]
        }
    }
}
</script>

<style scoped>
.child{
    background-color: rgb(145, 121, 91);
    height: auto;
    width: auto;
    padding: 30px;
    margin: 20px;
}
</style>