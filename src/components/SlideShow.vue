<script>
export default {
    data() {
        return {
            slideIndex: 1
        }
    },
    methods: {
        showSlides(n) {
            let i;
            let slides = document.getElementsByClassName("mySlides");
            let dots = document.getElementsByClassName("dot");
            if (n > slides.length) { this.slideIndex = 1 }
            if (n < 1) { this.slideIndex = slides.length }
            for (i = 0; i < slides.length; i++) {
                slides[i].style.display = "none";
            }
            for (i = 0; i < dots.length; i++) {
                dots[i].className = dots[i].className.replace(" active", "");
            }
            slides[this.slideIndex - 1].style.display = "block";
            dots[this.slideIndex - 1].className += " active";
        },
        plusSlides(n) {
            let myAdvance = this.slideIndex += n
            this.showSlides(myAdvance);
        },
        currentSlide(n) {
            this.showSlides(this.slideIndex = n);
        },
    }
}
</script>

<template>
    <!-- Slideshow container -->
    <div class="slideshow-container">

        <!-- Full-width images with number and caption text -->
        <div class="mySlides fade" style="display: block">
           
            <!-- <img src="img1.jpg" style="width:100%"> -->
            <div class="work-date">February 2017 - Present</div>
            <div class="work-name">CastleBranch</div>
            <div class="work-location">Wilmington, NC</div>
            <div class="work-position">UI/UX Manager</div>
            <div class="work-description">
                Manage team of Front End Designers and Developers to craft solutions for new features and functionality
                within the suite of CastleBrach product offerings, with a focus on usability and user flow. Develop new
                functionality and features within a Laravel stack using KendoUI, Vue.js, Vanilla Javascript, SASS and
                HTML. Work directly with Product Management to review business requirements and create functional
                requirements, as well as wireframes, mockups and clickable prototypes. Conduct key stakeholder meetings
                to review prototypes and present solutions for approval. Work directly with leadership to construct new
                SDLC process and implement within the engineering department. Interact with Quality Assurance department
                to review test plans and to help with feature testing. Manage all Front End development projects with
                emphasis on delivery dates, update leadership team on deliverables and the projects status.
            </div>
            <div class="text">Caption Text</div>
        </div>

        <div class="mySlides fade">
           
            <!-- <img src="img2.jpg" style="width:100%"> -->
            <div class="work-date">October 2015 - February 2017</div>
            <div class="work-name">Blue Acorn – eCommerce Web Agency</div>
            <div class="work-location">Location: Charleston, SC</div>
            <div class="work-position">Position: Front End Developer II</div>
            <div class="work-description">
                Use Magento eCommerce software to develop pixel perfect websites for high-end retailers. Work with
                Account Managers, System Architects and Senior Developers to create Business Requirement documentation
                used for Tech Designs and Estimations. Work as lead Front End Developer on website implementations and
                value creation projects. Extend the Magento framework by creating new modules, install and upgrade
                scripts and new themeing elements for desired functionality. Coordinate and manage work que and deliver
                assets to other departments in a timely manner. Work closely with Quality Assurance team members to test
                and fix defects. Participate in department meetings and training sessions. Work in an Agile development
                process and held accountable for story burn down. Attend daily standups and work with Scrum Masters to
                red flag potential problems and roadblocks. Work with integrity and continually striving to improve
                productivity and performance.</div>
            <div class="text">Caption Two</div>
        </div>

        <div class="mySlides fade">
            
            <!-- <img src="img3.jpg" style="width:100%"> -->
            <div class="work-date">October 2014 - October 2015</div>
            <div class="work-name">Jackson National Life Distributers</div>
            <div class="work-location">Location: Denver, CO</div>
            <div class="work-position">Position: Senior Web Designer (UI/UX) - Ecommerce</div>
            <div class="work-description">
                Use HTML5, CSS3, AJAX, Javascript and Jquery to develop cross department web projects for a variety of
                business sponsors. Work with Marketing and Creative departments to wireframe, mockup and implement new
                functionality and promotions across all corporate websites. Write and review requirements documentation
                to produce qualified estimates on new projects. Lead training and status meetings, working with multiple
                departments, in multiple locations, across the organization. Create process and procedure documentation
                for content managers with emphasis on reducing roadblocks and rework. Create and manage inhouse
                workflows to ensure all projects meet deadlines and expectations. Work with Compliance department to
                ensure web materials are designed and developed with limited risk and meet FINRA guidelines.</div>
            <div class="text">Caption Three</div>
        </div>

        <div class="mySlides fade">
            
            <!-- <img src="img3.jpg" style="width:100%"> -->
            <div class="work-date">October 2014 - October 2015</div>
            <div class="work-name">Jackson National Life Distributers</div>
            <div class="work-location">Location: Denver, CO</div>
            <div class="work-position">Position: Senior Web Designer (UI/UX) - Ecommerce</div>
            <div class="work-description">
                Use HTML5, CSS3, AJAX, Javascript and Jquery to develop cross department web projects for a variety of
                business sponsors. Work with Marketing and Creative departments to wireframe, mockup and implement new
                functionality and promotions across all corporate websites. Write and review requirements documentation
                to produce qualified estimates on new projects. Lead training and status meetings, working with multiple
                departments, in multiple locations, across the organization. Create process and procedure documentation
                for content managers with emphasis on reducing roadblocks and rework. Create and manage inhouse
                workflows to ensure all projects meet deadlines and expectations. Work with Compliance department to
                ensure web materials are designed and developed with limited risk and meet FINRA guidelines.</div>
            <div class="text">Caption Three</div>
        </div>

        <!-- Next and previous buttons -->
        <a class="prev" @click="plusSlides(-1)">&#10094;</a>
        <a class="next" @click="plusSlides(1)">&#10095;</a>
    </div>
    <br>

    <!-- The dots/circles -->
    <div style="text-align:center">
        <span class="dot active" @click="currentSlide(1)"></span>
        <span class="dot" @click="currentSlide(2)"></span>
        <span class="dot" @click="currentSlide(3)"></span>
        <span class="dot" @click="currentSlide(4)"></span>
        <!-- <span class="dot" onclick="currentSlide(3)"></span> -->
    </div>
</template>

<style lang="scss" scoped>
* {
    box-sizing: border-box
}

/* Slideshow container */
.slideshow-container {
    max-width: auto;
    position: relative;
    margin: auto;
}

/* Hide the images by default */
.mySlides {
    display: none;
}

/* Next & previous buttons */
.prev,
.next {
    cursor: pointer;
    position: absolute;
    top: 50%;
    width: auto;
    margin-top: -22px;
    padding: 16px;
    color: white;
    font-weight: bold;
    font-size: 18px;
    transition: 0.6s ease;
    user-select: none;
    background-color:#717171;
}
.prev {
    left: -50px;
    border-radius: 3px;
}
.next {
    right: -50px;
    border-radius: 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover,
.next:hover {
    background-color: rgba(0, 0, 0, 0.8);
}

/* Caption text */
.text {
    color: #f2f2f2;
    font-size: 15px;
    padding: 8px 12px;
    position: absolute;
    bottom: 8px;
    width: 100%;
    text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
    color: #f2f2f2;
    font-size: 12px;
    padding: 8px 12px;
    position: absolute;
    top: 0;
}

/* The dots/bullets/indicators */
.dot {
    cursor: pointer;
    height: 15px;
    width: 15px;
    margin: 0 2px;
    background-color: #bbb;
    border-radius: 50%;
    display: inline-block;
    transition: background-color 0.6s ease;
}

.active,
.dot:hover {
    background-color: #717171;
}

/* Fading animation */
.fade {
    animation-name: fade;
    animation-duration: 1.5s;
}

@keyframes fade {
    from {
        opacity: .4
    }

    to {
        opacity: 1
    }
}
</style>