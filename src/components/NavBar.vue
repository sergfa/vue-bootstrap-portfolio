<template>
    <nav class="navbar navbar-expand-md navbar-dark bg-dark p-3 fixed-top">
        <a href="#" class="navbar-brand text-uppercase">Perez Snow</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarBrand">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div id="navbarBrand" class="collapse navbar-collapse justify-content-end">
            <ul class="navbar-nav">
                <li  v-for="(item, index) in items" :key="index" class="nav-item" ><a :href="item.id" class="nav-link text-uppercase">{{item.title}}</a></li>
            </ul>
        </div>
    </nav>
</template>
<script>
export default {
    data () {
        return {
            items: [{id: '#banner', title: 'Home' },
                    {id: '#qualities', title: 'Qualities' },
                    {id: '#contact', title: 'Contact' },
                    {id: '#projects', title: 'Projects' },
                    {id: '#social', title: 'social'}]
        }
    }
}
</script>
