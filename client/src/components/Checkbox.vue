<template>
    <div>
        <h1>Technology</h1>
    <label for="ruby">Ruby</label>
    <input type="checkbox" value="ruby" id="ruby" v-model="technology">
    <label for="ror">Ruby On Rails</label>
    <input type="checkbox" value="ror" id="ror" v-model="technology">
    <label for="javaScript">JavaScript</label>
    <input type="checkbox" value="javaScript" v-model="technology" id="javaScript">
    <label for="nodeJS">Node JS</label>
    <input type="checkbox" value="nodeJS" v-model="technology" id="nodeJS">
    <label for="vueJS">Vue JS</label>
    <input type="checkbox" value="vueJS" v-model="technology" id="vueJS">

    <h4>Selected Technologies are {{ technology }}</h4>
    </div>
    <div>
        <h1>Profession</h1>

        <label for="student">Student</label>
        <input type="radio" value="student" name="profession" id="student" v-model="profession">
        <label for="freelancer">Freelancer</label>
        <input type="radio" value="freelancer" name="profession" id="freelancer" v-model="profession">
        <label for="job">Job</label>
        <input type="radio" value="job" name="profession" id="job" v-model="profession">

        <h4>Profession is {{ profession }}</h4>

    </div>


</template>
<script>
export default{
    name: 'CheckBox',
    data(){
        return{
        technology:[],
        profession: ''
        }
    }
}
</script>
<style></style>