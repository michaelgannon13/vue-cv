<template>
    <span>
        <home-hero></home-hero>
        <home-details></home-details>
        <home-skills></home-skills>
    </span>
</template>

<script>
import HomeHero from '@/components/HomeHero';
import HomeDetails from '@/components/HomeDetails';
import HomeSkills from '@/components/HomeSkills';

export default {
    name: 'home',
    components: {
        HomeHero, 
        HomeDetails,
        HomeSkills  
    }
};
</script>