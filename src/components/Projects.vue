<template>
    <section id="projects" class="py-5 bg-light">
        <div class="container">
            <div class="row">
                <div v-for="(item, index) in items" :key="index" class="col-sm-6 mb-3">
                    <img :src="item.image" :alt="item.name" class="img-fluid rounded">
                    <h2 class="my-3 text-capitalize font-weight-bold">{{item.name}}</h2>
                    <p class="text-secondary">{{item.description}}</p>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import image1 from '../assets/img/project1.jpg'
import image2 from '../assets/img/project2.jpg'
import image3 from '../assets/img/project3.jpg'
import image4 from '../assets/img/project4.jpg'

export default {
    data () {
        return {
            items: [{image: image1, name: 'Project 1', description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere dolores tempora quidem quia dolorum vitae unde ea beatae porro placeat!'},
            {image: image2, name: 'Project 2', description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere dolores tempora quidem quia dolorum vitae unde ea beatae porro placeat!'},
            {image: image3, name: 'Project 3', description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere dolores tempora quidem quia dolorum vitae unde ea beatae porro placeat!'},
            {image: image4, name: 'Project 4', description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere dolores tempora quidem quia dolorum vitae unde ea beatae porro placeat!'}]
        }
    }
}
</script>
