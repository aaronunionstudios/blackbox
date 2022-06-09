<script>
export default {
    data() {
        return {
            slideIndex: 1
        }
    },
    methods: {
        showSlides(n) {
            console.log('timer');
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
        }
        
    },
    mounted() {
        // setTimeout(this.plusSlides, 3000);
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
            <div class="work-date">September 2012 - October 2014</div>
            <div class="work-name">Creative Services LLC.</div>
            <div class="work-location">Location: Charlotte, NC</div>
            <div class="work-position">Position: Interactive Director</div>
            <div class="work-description">
                Use HTML5, CSS3, AJAX, Jquery and PHP to develop custom website solutions for national sales network. Conduct client meetings to discuss frontend and backend functionality with emphasis on useability. Use XHTML, MySQL and PHP to develop dynamic Ecommerce websites that drive sales. Develop and maintain custom WordPress development framework, with emphasis on browser and device compatibility. Oversee design concepting to ensure the end results match customer expectations. Create custom jQuery and AJAX web applications to deliver a streamlined user experience. Develop custom PHP and MySQL scripts for custom database functionality. Manage daily work schedule and oversee programming department with emphasis on deadlines. Conduct weekly programming department meetings to leverage team assets for complicated buildouts. Create custom tutorial and training materials for end users and manage client/sales training. Manage hosting department with emphasis on website/email security, software updates and new website launches. Work with server team to trouble shoot problematic websites, broken functionality and hacked/malicious website issues.</div>
            <div class="text">Caption Three</div>
        </div>

        <div class="mySlides fade">
            
            <!-- <img src="img3.jpg" style="width:100%"> -->
            <div class="work-date">January 2011 - September 2012</div>
            <div class="work-name">Union Studios LLC.</div>
            <div class="work-location">Location: Marshville, NC</div>
            <div class="work-position">Position: Creative Director/Interactive Director</div>
            <div class="work-description">
                Develop custom website solutions on a variety of CMS frameworks. Use HTML, CSS, Jquery and PHP to create WordPress Plugins and Themes for custom funcionality with emphasis on useablility. Run client meetings to discuss website goals, sitemaps and review interactive proofs. Create and deliver HTML email newsletters, marketing campaigns and announements, monitor delivery results and create reports for marketing review. Incorporate Google Analytics and Webmaster Tools into websites, add blog functionality into existing websites and develop blog campaigns to boost SEO rankings.</div>
            <div class="text">Caption Three</div>
        </div>

        <div class="mySlides fade">
            
            <!-- <img src="img3.jpg" style="width:100%"> -->
            <div class="work-date">September 2008 - January 2011</div>
            <div class="work-name">Affinity 4, Inc. and Beliefnet.com</div>
            <div class="work-location">Location: Norfolk VA</div>
            <div class="work-position">Position: Senior Graphic/Web Designer</div>
            <div class="work-description">
                Use HTML, CSS, PHP and JavaScript to build new product ordering website for NPO business unit. Build custom landing pages in HTML and CSS for business partners. Design and develop dynamic PHP web application to dynamically generate marketing materials. Helped coordinate BN Media’s acquisition of BELIEFNET.com, website with over 3 million monthly unique visitors. Manage and maintain corporate websites with updated content and new marketing incentives. Create HTML email newsletters and marketing incentives. Develop HTML interactive sales material pages for new product launches and promotional sales. Developed custom Social Media landing pages and tied into exisiting Social Media platforms.</div>
            <div class="text">Caption Three</div>
        </div>

        <div class="mySlides fade">
            
            <!-- <img src="img3.jpg" style="width:100%"> -->
            <div class="work-date">September 2004 - September 2008</div>
            <div class="work-name">PlayPower, Inc.</div>
            <div class="work-location">Location: Huntersville, NC</div>
            <div class="work-position">Position: Graphic/Web Designer</div>
            <div class="work-description">
                Use HTML and CSS to rebrand 5 corporate websites and buildout in a CMS framework. Develop animated banner ads for product promotion through website ad campaigns. Work with sales force to develop PHP and MySQL password protected online marketing material database. Develop monthly e-newsletter in HTML and CSS for delivery to customer email list. Manage in-house hosted websites on Windows IIS Server. Develop custom HTML website landing pages for tracking marketing advertising efforts.</div>
            <div class="text">Caption Three</div>
        </div>

        <div class="mySlides fade">
            
            <!-- <img src="img3.jpg" style="width:100%"> -->
            <div class="work-date">September 1997 - October 2003</div>
            <div class="work-name">ACI Design Inc.</div>
            <div class="work-location">Location: Charlotte, NC</div>
            <div class="work-position">Position: Exhibit Designer</div>
            <div class="work-description">
                Work with sales staff and clients to create successful tradeshow strategies. Design and develop tradeshow exhibits with emphasis toward goals and budgets. Print and prepare large format inkjet prints for displays. Train and manage production artists. Install and manage tradeshow exhibit installations.</div>
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
        <span class="dot" @click="currentSlide(5)"></span>
        <span class="dot" @click="currentSlide(6)"></span>
        <span class="dot" @click="currentSlide(7)"></span>
        <span class="dot" @click="currentSlide(8)"></span>
        <!-- <span class="dot" onclick="currentSlide(3)"></span> -->
    </div>
</template>

<style lang="scss" scoped>
.work-date {
    font-size:0.8rem;
}
.work-name {
    font-size:1.4rem;
    font-weight:bold;
}
.work-location {
    font-size:0.9rem;
}
.work-position {
    font-size:1rem;
    font-style:italic;
    padding-bottom: 10px;
    font-weight:bold;
}
.work-description {
    font-size:1rem;
}
.slideshow-container {
    padding: 0 20px;
}

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