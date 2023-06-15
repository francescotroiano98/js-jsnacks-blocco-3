<template>
    <div>
        <nav>
            <ul>
                <li v-for="link in links">{{ link }}</li>
                
            </ul>
        </nav>
    </div>
</template>

<script>
export default {

    name: 'AppHeader',

    data(){
        return{

            links :[
                'gino',
                'ginetta',
                'gina',
                'ginettina'
            ]

        }
    }
    
}
</script>
<style lang="scss" scoped>

ul{
    display: flex;

    li{
        margin-right: 2rem;
    }
}
    
</style>