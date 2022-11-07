<template>
    <NavbarGeneral></NavbarGeneral>
    <div class="d-flex">
        <div class="col-4">
            <EntryList></EntryList>
        </div>
        <div class="col">
            <router-view></router-view>
        </div>
    </div>
</template>

<script>
import { defineAsyncComponent } from 'vue';


export default {
    components:{
    NavbarGeneral: defineAsyncComponent(() => import('../components/NavbarGeneral.vue')),
    EntryList: defineAsyncComponent(() => import('../components/EntryList.vue')),
    
    }
}
</script>