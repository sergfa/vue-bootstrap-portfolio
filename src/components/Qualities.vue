<template>
    <section id="qualities" class="bg-primary py-5 text-light">
        <div class="container">
            <div class="row align-items-center">
                <div v-for="(item, index) in items" :key="index" class="col-md-6 col-lg-4 d-flex mb-3">
                    <i class="fas fa-3x align-self-center" :class="'fa-'+item.icon"></i>
                    <div class="quality ml-4 text-left">
                        <h2 class="text-uppercase mb-3">{{item.name}}</h2>
                        <p>{{item.description}}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    data () {
        return {
            items: [{icon: 'wrench', name: 'Hard Work', description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit molestias odio vero maxime fuga, doloremque magnam vel enim iusto alias?'},
            {icon: 'graduation-cap', name: 'Learning', description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit molestias odio vero maxime fuga, doloremque magnam vel enim iusto alias?'},
            {icon: 'handshake', name: 'Reliable', description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit molestias odio vero maxime fuga, doloremque magnam vel enim iusto alias?'}] 
        }
    }
}
</script>
