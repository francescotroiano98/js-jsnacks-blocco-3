<template>
    <div>
        <nav>
            <ul>
                
                <NavLink  v-for="link in links" :linkElements="link"/>
                
            </ul>
        </nav>
    </div>
</template>

<script>
import NavLink from '../components/NavLink.vue'

export default {

    name: 'AppHeader',

    data(){
        return{

            links :[
                'gino',
                'ginetta',
                'gina',
                'ginettina'
            ],
            components:  {
                NavLink
            }

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