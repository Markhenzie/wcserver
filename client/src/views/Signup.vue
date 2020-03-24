<template>
    <div class = 'signup_con'>
        <div class = 'row'>
            <div id="column_main_signup" class = 'col-md-4'>
                <h2>Create an Account</h2>
                <form @submit.prevent = 'registerUser'>
                    <div class = 'form-group'>
                        <div class = "form-group">
                            <label for = 'First Name'> First Name </label>
                            <input type = 'text' name = 'fname' id = 'fname' placeholder = 'Enter First Name' v-model = 'fname' class="form-control"/>
                        </div>

                        <div class = "form-group">
                            <label for = 'Middle Initial'> Middle Name </label>
                            <input type = 'text' name = 'mid' id = 'mid' placeholder = 'Enter Middle Initial' v-model = 'mid' class="form-control"/>
                        </div>

                        <div class = "form-group">
                            <label for = 'Last Name'> Last Name </label>
                            <input type = 'text' name = 'lname' id = 'lname' placeholder = 'Enter Last Name' v-model = 'lname' class="form-control"/>
                        </div>

                        <div class = "form-group">
                            <label for = 'Last Name'> Contact Number </label>
                            <input type = 'text' name = 'num' id = 'lname' placeholder = 'Enter Contact Number' v-model = 'num' class="form-control"/>
                        </div>
                        
                        <div class = "form-group">
                            <label for = 'Birth Date'> Birthdate </label>
                            <input type = 'text' name = 'bday' id = 'bday' placeholder = 'Enter Birth Date' v-model = 'bday' class="form-control"/>
                        </div>

                        <div class = "form-group">
                            <label for = 'Address'> Address </label>
                            <input type = 'text' name = 'Address' id = 'Address' placeholder = 'Enter address' v-model = 'Address' class="form-control"/>
                        </div>

                        <div class = "form-group">
                            <label for = 'Email Address'> Email Address </label>
                            <input type = 'email' name = 'Email' id = 'Address' placeholder = 'Enter Email Address' v-model = 'Email' class="form-control"/>
                        </div>

                        <div class = "form-group">
                            <label for = 'Username'> Username </label>
                            <input type = 'text' name = 'user' id = 'user' placeholder = 'Enter Username' v-model = 'user' class="form-control"/>                                                
                        </div>

                        <div class = "form-group">
                            <label for = 'Password'> Password </label>
                            <input type = 'password' name = 'Password' id = 'Password' placeholder = 'Enter Password' v-model = 'Password' class="form-control"/>
                        </div>
                        
                        <button type="submit" class="regbtn">Register</button>
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
                mid: '',
                lname: '',
                Adress: '',
                bday:'',
                Email:'',
                user: '',
                Pass:''
            }
        },
        methods:
        {
            registerUser()
            {
                if (this.fname==='')
                {
                    alert('Please enter your first name:')
                }
            }
        }
    }
</script>
<style>

</style>