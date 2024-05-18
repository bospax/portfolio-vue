<script setup>
	import meImage from '@/assets/img/me.jpg';
</script>

<template>
	<main>
        <h1><span>Hello.</span><br>I’m Jose.</h1>

        <h2>
            I’m a <span>Fullstack Developer</span> & <span>App Enthusiast</span>.
        </h2>

        <img class="profile" :src="meImage" alt="">

        <p>
            With over 5 years of software development experience.<br>
            Previously Web Application Developer at <a href="#">RDF Feeds, Livestock & Food Inc</a>.<br>
            Previously Wordpress & PHP Developer at <a href="#">IConcept Global Advertising</a>.<br>
            Previously Multimedia Officer at <a href="#">VTG Travel and Tours</a>.
        </p>


        <p>Reach me via 
            <a href="mailto:josedpachecojr@gmail.com">Email</a>, 
            <!-- <a href="#">GitHub</a>,  -->
            <a target="_blank" href="https://www.linkedin.com/in/josepachecojr">LinkedIn</a>.
            <br>Full name is Jose Pacheco Jr. Nice to meet you.
        </p>

        <section class="skills">
            <h2>Tech Stacks.🔥 <p>List of my Programming Technologies and Toolsets:</p></h2>
            
            <div class="grid-container">
                <div class="grid-item">
                    <img src="./assets/img/tech/laravel.jpg" alt="">
                    <p>Laravel</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/php.png" alt="">
                    <p>PHP</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/rest.jpg" alt="">
                    <p>REST</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/pusher.png" alt="">
                    <p>Pusher</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/axios.png" alt="">
                    <p>Axios</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/ajax.png" alt="">
                    <p>Ajax</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/websocket.png" alt="">
                    <p>WebSocket</p>
                </div>
            </div>

            <hr class="style-three">

            <div class="grid-container">
                <div class="grid-item">
                    <img src="./assets/img/tech/vue.jpg" alt="">
                    <p>VueJS</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/pinia.png" alt="">
                    <p>Pinia</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/vuex.png" alt="">
                    <p>Vuex</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/quasar.png" alt="">
                    <p>Quasar</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/tailwind.png" alt="">
                    <p>Tailwind</p>
                </div>
            </div>

            <hr class="style-three">

            <div class="grid-container">
                <div class="grid-item">
                    <img src="./assets/img/tech/html.png" alt="">
                    <p>HTML</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/css.png" alt="">
                    <p>CSS</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/javascript.png" alt="">
                    <p>JS</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/scss.png" alt="">
                    <p>SCSS</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/bootstrap.png" alt="">
                    <p>Bootstrap</p>
                </div>
            </div>

            <hr class="style-three">

            <div class="grid-container">
                <div class="grid-item">
                    <img src="./assets/img/tech/mysql.png" alt="">
                    <p>MySQL</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/firebase.png" alt="">
                    <p>Firebase</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/git.png" alt="">
                    <p>GIT</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/github.png" alt="">
                    <p>Github</p>
                </div>
            </div>

            <hr class="style-three">

            <div class="grid-container">
                <div class="grid-item">
                    <img src="./assets/img/tech/shopify.jpg" alt="">
                    <p>Shopify</p>
                </div>
                <div class="grid-item">
                    <img src="./assets/img/tech/wordpress.png" alt="">
                    <p>Wordpress</p>
                </div>
            </div>
        </section>

        <section class="projects">
            <h2>Projects.❤️ <p>List of my Experimental and Major Projects:</p></h2>
            
            <div class="grid-container">
                <div 
                    data-bs-toggle="offcanvas" 
                    data-bs-target="#offcanvasExample" 
                    aria-controls="offcanvasExample"
                    class="grid-item" 
                    style="background: url('./assets/img/projects/freshoptions.png') center/cover no-repeat; filter: grayscale(1);"
                >
                    <p>SEDAR RECRUITMENT</p>
                </div>
                <div class="grid-item"></div>
                <div class="grid-item"></div>
                <div class="grid-item"></div>
                <div class="grid-item"></div>
                <div class="grid-item"></div>
                <div class="grid-item"></div>
                <div class="grid-item"></div>
                <div class="grid-item"></div>
            </div>
        </section>
          
        <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasExample" aria-labelledby="offcanvasExampleLabel">
            <div class="offcanvas-header">
                <h5 class="offcanvas-title" id="offcanvasExampleLabel"></h5>
                <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
            </div>
            <div class="offcanvas-body">
                <div>
                    <h3>SEDAR</h3>
                    <p>Employee Management System</p>
                    <a href="" target="_blank"><img src="./assets/img/projects/freshoptions.png" alt=""></a>
                    <p>👉 <a href="http://localhost/portfolio/" target="_blank">http://localhost/portfolio/</a></p>
                    <p>HR Management system for managing Employee Data, Form Requests, KPI / Grade Evaluation, Masterlists, User Account Management and for storing company files and documents.</p>
                    <p>Features:</p>
                    <ul>
                        <li>Employee Management & Registration</li>
                        <li>Manpower & Evaluation form Requests</li>
                        <li>Delete, Edit, Update Masterlists</li>
                        <li>Request & Approval system</li>
                    </ul>
                    <p>🔥 Made with: Laravel, Vue, MySQL, Bootstrap, HTML, CSS, JS</p>
                </div>
            </div>
        </div>
    </main>
</template>

<style scoped>

</style>
