<template lang="">
    <div class="Contact">
        <form>
        <label for="fullname">Fullname</label>: 
        <input type="text" placeholder="Fullname..." v-model="fullname"><br><br>
        <label for="email">Email</label>: 
        <input type="email" placeholder="Email..." v-model="email"><br><br>
        <label for="age">Age</label>: 
        <input type="number" placeholder="Age..." v-model="age"><br><br>
        <label for="dob">DOB</label>: 
        <input type="date" placeholder="DOB..." v-model="dob"><br><br>
        <input type="submit" id="submit" placeholder="Submit" v-on:click.prevent="submit">
    </form>   
    </div>
</template>
<script>
export default {
    methods: {
        greet: function(event){
            alert(event.target.tagName);
        }
    }
}
</script>
<style lang="">
    
</style>