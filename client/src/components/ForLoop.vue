<template>
    <h1>For Loop</h1>
    <ul>
        <li v-for="post in post" :key="post.id">Name is : {{ post.name }} and email is : {{ post.email   }}</li>
    </ul>

    <!-- <p>{{ API_URL }}</p> -->


</template>
<script>
export default{
    name: 'ForLoop',
    data(){
        return{
            post:[
            {
                name: 'name1',
                email: 'name1@test.com',
                phone: '111-111-1111'
            },
            {
                name: 'name2',
                email: 'name2@test.com',
                phone: '111-111-1111'
            },
            {
                name: 'name3',
                email: 'name3@test.com',
                phone: '111-111-1111'
            },
            {
                name: 'name4',
                email: 'name4@test.com',
                phone: '111-111-1111'
            },
            {
                name: 'name5',
                email: 'name5@test.com',
                phone: '111-111-1111'
            },
            {
                name: 'name6',
                email: 'name6@test.com',
                phone: '111-111-1111'
            },
        ]
        }
    },
}
</script>
<style></style>