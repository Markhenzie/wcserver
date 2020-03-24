<template>
    <div class = 'login_con'>
        <div class = 'row'>
            <div class = 'col-md-3'>
                <h1>Log In</h1>
                <form @submit.prevent = 'registerUser'>
                    <div class = 'form-group'>

                        <div class = "form-group-two">
                            <label>Email Address</label>
                            <input type = 'text' name = 'email' id = 'email' placeholder = 'Email Address' v-model = 'email' class="form-control"/>
                            <br>
                        </div>

                        <div class = "form-group-two">
                            <label>Password</label>
                            <input type = 'password' name = 'pass' id = 'pass' placeholder = 'Password' v-model = 'pass' class="form-control"/>
                        </div>
                        <br>
                        <button type="submit" class="loginbtn">Log In</button>
                        <button type="button" class="cancelbtn">Cancel</button>
                        
                        
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>
<script>

//import axios from 'axios'
//import router from '../router'
export default{
        data (){
            return{

                fname: '',
                Mname: '',
                lname: '',
                Adress: '',
                DOB:'',
                email:'',
                user: '',
                pass:''
            }
        },
        methods:
        {
            registerUser()
            {
                if (this.email==='')
                {
                    alert('Please enter your email address.')
                }
            }
        }
    }
</script>
<style>

</style>