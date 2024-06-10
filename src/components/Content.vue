<script setup lang="ts">
    import { ref } from 'vue';
    import { data } from '../Data';
    
</script>

<template>
    <div class="container-wap">
        <div class="container">
            <div>
                <h1>Photo Cards: </h1>
            </div>
            <div v-for="(item, index) in data" :key="index" class="row-col">
                <div class="col-xl-2 col-lg-3 col-md-3 col-sm-4">
                    <div class="card">
                        <img class="card-img-top" :src="item.image" :alt="item.title">
                        <div class="card-body">
                            <p>{{ item.title }}</p>
                        </div>
                    </div>
                </div>
              </div>
        </div>
    </div>
</template>