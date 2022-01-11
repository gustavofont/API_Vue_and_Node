<template>
    <div>
        <div class="container">
            <h1 class="title">Register</h1>
            <div class="box">
                <div class="field">
                    <label class="label">Name</label>
                    <div class="control">
                        <input class="input" type="text" placeholder="Gustavo Machado" v-model="name">
                    </div>
                </div>

                <div class="field">
                    <label class="label">Email</label>
                    <div class="control">
                        <input class="input" type="email" placeholder="e.g. alex@example.com" v-model="email">
                    </div>
                </div>

                <div class="field">
                    <label class="label">Password</label>
                    <div class="control">
                        <input class="input" type="password" placeholder="********" v-model="password">
                    </div>
                </div>

                <button class="button is-primary" @click="register">Register</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            name : '',
            password : '',
            email : ''
        }
    },
    methods: {
        register(){
            console.log('name = ' + this.name)
            console.log('email = ' + this.email)
            console.log('password = ' + this.password)
        }
    }
}
</script>

<style>

</style>