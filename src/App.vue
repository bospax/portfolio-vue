<template>
	<main>
        <h1><span>Hello.</span><br>I’m Jose.</h1>

        <h2>
            I’m a <span>Fullstack Developer</span> & <span>App Enthusiast</span>.
        </h2>

        <img class="profile" :src="meImage" alt="">

        <p>
            With over 5 years of software development experience.<br>
            Previously Project Based Web Developer at <a href="#">RDF Feeds, Livestock & Food Inc</a>.<br>
            Previously Junior Web App Developer at <a href="#">RDF Feeds, Livestock & Food Inc</a>.<br>
            Previously Wordpress & PHP Developer at <a href="#">IConcept Global Advertising</a>.<br>
            Previously Multimedia Officer at <a href="#">VTG Travel and Tours</a>.
        </p>


        <p>Reach me via 
            <a href="mailto:josedpachecojr@gmail.com">Email</a>, 
            <!-- <a href="#">GitHub</a>,  -->
            <a target="_blank" href="https://www.linkedin.com/in/josepachecojr">LinkedIn</a>.
            <br>You may also review my <a target="_blank" href="https://drive.google.com/file/d/1UKI-U9OmIqfSniq3J56LGcQbeJltfZK1/view?usp=sharing">CV</a>.
            <br>Full name is Jose Pacheco Jr. Nice to meet you.
        </p>

        <section class="skills">
            <h2>Tech Stacks.🔥 
                <p>Here are my diverse arsenal of programming technologies and toolsets, over years of hands-on experience. From mastering frontend frameworks like VueJS to leveraging the power of Laravel for backend development, my skill set encompasses a wide range of tools designed to create seamless and efficient web applications. </p>
            </h2>
            
            <TechStacks :items="TechStackItems.server"/>

            <hr class="style-three">

            <!-- <TechStacks :items="TechStackItems.frameworks"/>

            <hr class="style-three"> -->

            <TechStacks :items="TechStackItems.client"/>

            <hr class="style-three">

            <TechStacks :items="TechStackItems.database"/>

            <hr class="style-three">

            <TechStacks :items="TechStackItems.cms"/>
        </section>

        <section class="projects">
            <h2>Projects.❤️ 
                <p>Browse through my collection of experimental and major projects. This portfolio showcases my dedication to pushing the limits and creating impactful solutions in the world of software development.</p>
            </h2>
            
            <ProjectList @projectSelected="handleProjectSelected" :items="ProjectListItems.projects" />
        </section>
          
        <ProjectDrawer :item="selectedProject" />
    </main>
</template>

<script setup>
    import TechStacks from '@/components/TeckStack.vue';
    import ProjectList from '@/components/ProjectList.vue';
    import ProjectDrawer from '@/components/ProjectDrawer.vue';
    import meImage from '@/assets/img/me.jpg';
    import TechStackItems from '@/data/TechStacks';
    import ProjectListItems from '@/data/ProjectList';
    import { ref } from 'vue';

    const selectedProject = ref({});

    const handleProjectSelected = (item) => {
        selectedProject.value = item;
    };
</script>

<style scoped>

</style>
