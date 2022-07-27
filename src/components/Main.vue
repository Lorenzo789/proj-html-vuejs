<template>
    <main class="container-fluid">

        <!-- NAVBAR -->
        <NavBarMain />
        <!-- NAVBAR -->

        <!-- SECTION INVESTING -->
        <SectionInvestingMain v-for="(element, index) in  sectionInvesting" :key="index" :title="element.title"
            :subTitle="element.subTitle" 
        />
        <!-- SECTION INVESTING -->

        <!-- SECTION CARD PRESENTATION -->
        <div class="container p-2 my-5">
            <div class="row my-5">
                <div class="ms_card">
                    <div>
                        <i class="fa-solid fa-earth-europe ms_fs_icon"></i>
                        <h5>Worldwide Recognize</h5>
                        <p>Our online courses certificates can be used around the world and also in most popular
                            universities and companies
                        </p>
                    </div>
                </div>
                <div class="ms_card">
                    <div>
                        <i class="fa-solid fa-tv ms_fs_icon"></i>
                        <h5>Mostly online Learning (sd)</h5>
                        <p>Masterstudy online certificates can be obtained in a range of specialized areas and typically
                            take about a year to complete
                        </p>
                    </div>
                </div>
                <div class="ms_card">
                    <div>
                        <i class="fa-solid fa-calendar-check ms_fs_icon"></i>
                        <h5>Graduate in as little as 1 Year</h5>
                        <p>Online post graduate certificates are a popular way to develop your professional
                            qualifications of Masterstudy
                        </p>
                    </div>
                </div>
            </div>
        </div>
        <!-- SECTION CARD PRESENTATION -->

        <!-- SECTION COURSES TYPE -->
        <SectionListCoursesMain />
        <!-- SECTION COURSES TYPE -->

        <!-- SECTION LEARNING -->
        <div class="container-fluid ms_bg">
            <SectionLearningMain v-for="(element, index) in sectionLearning" :key="index"
                :title="element.title"
                :subTitle="element.subTitle"
            />
        </div>
        <!-- SECTION LEARNING -->

        <!-- SECTION RECENT COURSES -->
        <div class="container-fluid p-5 my-5 position-relative">

            <h1 class="text-center mb-5">Recent courses</h1>

            <ul class="text-center mb-5">
                <CoursesGenre v-for="(element, index) in genreCourse" :key="index"
                    :nameGenre="element.genre"
                    :selected="element.selected"
                />
            </ul>

            <!-- COMPONENT CARD CORSI -->
            <div class="d-flex flex-wrap justify-content-between">
                <CardGenre v-for="(card, index) in genreCard" :key="index"
                    :imgUrl="card.imgUrl"
                    :description="card.description"
                    :title="card.title"
                    :hour="card.hour"
                    :stars="card.stars"
                    :numberStars="card.numberStars"
                    :cost="card.cost"
                    :oldCost="card.oldCost"
                    :new="card.new"
                    :hot="card.hot"
                    :special="card.special"
                />
            </div>
            <!-- COMPONENT CARD CORSI -->

            <!-- TENDINA LATERALE -->
            <div class="p-3 border text-center position-absolute bottom-0 end-0 shadow p-3 mb-5 bg-body rounded">
                <div><i class="fa-solid fa-tv p-2"></i></div>
                <div><i class="fa-solid fa-futbol p-2"></i></div>
                <div><i class="fa-solid fa-wrench p-2"></i></div>
                <div><i class="fa-solid fa-cart-shopping p-2"></i></div>
                <div><i class="fa-solid fa-mobile-screen p-2"></i></div>
            </div>
            <!-- TENDINA LATERALE -->

            <div class="text-center">
                <ButtonComponent v-for="(text, index) in mainBtnText" :key="index"
                    :mainText="text.mainText"
                />
            </div>
        </div>
        <!-- SECTION RECENT COURSES -->

        <div class="container p-2 my-5">
            <h1>Titolo</h1>
            <p>Testo</p>
            <div class="row">
                <div class="col-3">dato</div>
                <div class="col-3">dato</div>
                <div class="col-3">dato</div>
                <div class="col-3">dato</div>
            </div>
        </div>

        <div class="container p-2 my-5">
            <h1>Titolo</h1>
            <p>Testo</p>
            <label for="">email</label>
            <!-- COMPONENT SEARCHBAR -->
            <input type="text" placeholder="Search courses">
            <button>Cerca</button>
            <!-- COMPONENT SEARCHBAR -->
        </div>

        <div class="container p-2 my-5">
            <div class="row">
                <h1>Titolo</h1>
                <p>Testo</p>
                <div class="col-2">
                    <img src="../assets/images/photo-1416339134316-0e91dc9ded92-scaled-272x161.jpeg" alt="">
                    <p>descrizione</p>
                    <h6>Titolino</h6>
                    <span>ore</span>
                    <span>costo</span>
                </div>

                <div class="col-2">
                    <img src="../assets/images/photo-1416339134316-0e91dc9ded92-scaled-272x161.jpeg" alt="">
                    <p>descrizione</p>
                    <h6>Titolino</h6>
                    <span>ore</span>
                    <span>costo</span>
                </div>

                <div class="col-2">
                    <img src="../assets/images/photo-1416339134316-0e91dc9ded92-scaled-272x161.jpeg" alt="">
                    <p>descrizione</p>
                    <h6>Titolino</h6>
                    <span>stelline</span>
                    <span>costo</span>
                </div>

                <div class="col-2">
                    <img src="../assets/images/photo-1416339134316-0e91dc9ded92-scaled-272x161.jpeg" alt="">
                    <p>descrizione</p>
                    <h6>Titolino</h6>
                    <span>stelline</span>
                    <span>costo</span>
                </div>

                <div class="col-2">
                    <img src="../assets/images/photo-1416339134316-0e91dc9ded92-scaled-272x161.jpeg" alt="">
                    <p>descrizione</p>
                    <h6>Titolino</h6>
                    <span>ore</span>
                    <span>costo</span>
                </div>

                <div class="col-2">
                    <img src="../assets/images/photo-1416339134316-0e91dc9ded92-scaled-272x161.jpeg" alt="">
                    <p>descrizione</p>
                    <h6>Titolino</h6>
                    <span>ore</span>
                    <span>costo</span>
                </div>

                <div>carosello</div>
            </div>
        </div>

        <div class="container p-2 my-5">
            <div class="row">
                <div class="col-6">
                    <div class="col-6">
                        <h6>Titolo</h6>
                        <p>Testo</p>
                        <!-- COMPONENT BUTTON -->
                        <button>JOIN</button>
                        <!-- COMPONENT BUTTON -->
                    </div>
                    <div class="col-6">
                        <img src="" alt="">
                    </div>
                </div>
                <div class="col-6">
                    <div class="col-6">
                        <h6>Titolo</h6>
                        <p>Testo</p>
                        <!-- COMPONENT BUTTON -->
                        <button>JOIN</button>
                        <!-- COMPONENT BUTTON -->
                    </div>
                    <div class="col-6">
                        <img src="" alt="">
                    </div>
                </div>
            </div>
        </div>

        <div class="container-fluid p-2 my-5">
            <div class="container p-2">
                <h1>Titotlo</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Expedita aut molestiae beatae dolorem, sequi
                    odio rem facilis nemo ex exercitationem deleniti excepturi, quasi totam, voluptatibus officia
                    eveniet laboriosam ipsa ut.</p>
                <p>info</p>
            </div>
        </div>
    </main>
</template>

<script>
import NavBarMain from "./ComponentsMain/NavBarMain.vue";
import SectionInvestingMain from "./ComponentsMain/SectionInvestingMain.vue";
import SectionListCoursesMain from "./ComponentsMain/SectionListCoursesMain.vue";
import SectionLearningMain from "./ComponentsMain/SectionLearningMain.vue";
import CoursesGenre from "./ComponentsMain/CoursesGenre.vue";
import CardGenre from "./ComponentsMain/CardGenre.vue";
import ButtonComponent from "./ComponentCommon/ButtonComponent.vue";

export default {
    data: function () {
        return {
            sectionInvesting: [
                {
                    title: 'Start Investing in You',
                    subTitle: 'With over 1200 courses in 18 subjects, youre guaranteed to find something thats right for you',
                },
            ],
            sectionLearning: [
                {
                    title: 'Limitless learning, more possibilities',
                    subTitle: 'Online courses open the opportunity for learning to almost anyone, regardless of their scheduling commitments.',
                }
            ],
            genreCourse: [
                {
                    genre: 'All Categories',
                    selected: true,
                },
                {
                    genre: 'Art',
                    selected: false,
                },
                {
                    genre: 'Exercise',
                    selected: false,
                },
                {
                    genre: 'Material Design',
                    selected: false,
                },
                {
                    genre: 'Music',
                    selected: false,
                },
                {
                    genre: 'Photography',
                    selected: false,
                },
                {
                    genre: 'Software Development',
                    selected: false,
                },
            ],
            genreCard: [
                {
                    imgUrl: require('../assets/images/photo-1461749280684-dccba630e2f6-272x161.jpeg'),
                    description: 'Apache>',
                    title: 'Web Coding and Apache Basics',
                    hour: '6 hours',
                    cost: 'Free',
                    new: false,
                    hot: false,
                    special: false,
                },
                {
                    imgUrl: require('../assets/images/cat_2-272x161.jpg'),
                    description: 'Art>',
                    title: 'Real Things Art Painting By Jason Ni',
                    hour: '6 hours',
                    oldCost: '$60',
                    cost: '$45',
                    new: true,
                    hot: false,
                    special: false,
                },
                {
                    imgUrl: require('../assets/images/course-preview-272x161.jpg'),
                    description: 'Software Development>',
                    title: 'Basics of Masterstudy',
                    hour: '',
                    stars: '★★★★★',
                    numberStars: '5',
                    cost: 'Free',
                    new: false,
                    hot: true,
                    special: false,
                },
                {
                    imgUrl: require('../assets/images/photo-1496307042754-b4aa456c4a2d-272x161.jpeg'),
                    description: 'Electronic>',
                    title: 'How To Be a DJ? Make Electronic Music',
                    hour: '',
                    stars: '★★★★★',
                    numberStars: '5',
                    oldCost: '$59',
                    cost: '$49',
                    new: false,
                    hot: false,
                    special: true,
                },
                {
                    imgUrl: require('../assets/images/photo-1416339134316-0e91dc9ded92-scaled-272x161.jpeg'),
                    description: 'Communication>',
                    title: 'Design Instrument For Communication',
                    hour: '6 hours',
                    cost: 'Free',
                    new: false,
                    hot: false,
                    special: false,
                },
                {
                    imgUrl: require('../assets/images/cathryn-lavery-67852-unsplash-272x161.jpg'),
                    description: 'Art>',
                    title: 'Make your Concept Right and Beautiful',
                    hour: '6 hours',
                    cost: '$70',
                    new: false,
                    hot: false,
                    special: false,
                },
                {
                    imgUrl: require('../assets/images/photo-1475452779376-caebfb988090-272x161.jpeg'),
                    description: 'Bicycling>',
                    title: 'Road Bike Manual or How to Be a Champion',
                    hour: '6 hours',
                    cost: '$20',
                    new: false,
                    hot: false,
                    special: false,
                },
                {
                    imgUrl: require('../assets/images/cristian-grecu-762012-unsplash-min-scaled-272x161.jpg'),
                    description: 'Documentary>',
                    title: 'How to Make Beautiful Landscape Photos?',
                    hour: '6 hours',
                    cost: '$60',
                    new: false,
                    hot: false,
                    special: false,
                },
                {
                    imgUrl: require('../assets/images/landscape-272x161.jpg'),
                    description: 'Art>',
                    title: 'Let`s paint Van Gogh`s Starry Night',
                    hour: '6 hours',
                    cost: '$79',
                    new: false,
                    hot: false,
                    special: false,
                },
                {
                    imgUrl: require('../assets/images/12345-1-272x161.png'),
                    description: 'Nvidia>',
                    title: 'Nvidia and UE4 Technologies Practice',
                    hour: '',
                    stars: '★★★★★',
                    numberStars: '5',
                    cost: 'Free',
                    new: false,
                    hot: false,
                    special: true,
                },
                {
                    imgUrl: require('../assets/images/jakob-owens-198234-unsplash-min-1-272x161.png'),
                    description: 'Art>',
                    title: 'How to Work with Legendary Red camera?',
                    hour: '6 hours',
                    cost: 'Free',
                    new: false,
                    hot: false,
                    special: true,
                },
                {
                    imgUrl: require('../assets/images/promo_tf-272x161.jpg'),
                    description: 'Software Development>',
                    title: 'MasterStudy Mobile LMS App',
                    hour: '2 hours',
                    cost: 'Free',
                    new: false,
                    hot: false,
                    special: false,
                },
            ],
            mainBtnText: [
                {
                    mainText: 'Show All',
                }
            ],
        };
    },
    components: { NavBarMain, SectionInvestingMain, SectionListCoursesMain, SectionLearningMain, CoursesGenre, CardGenre, ButtonComponent }
}
</script>

<style lang="scss" scoped>
@import'../styles/variables.scss';

    .ms_card:hover{
        margin-top: -50px;
        transition: margin-top 1s;
        cursor: pointer;
    }

    .ms_card{
        width: calc(100% / 3 - 25px);
        margin-right: 25px;

        div{
            background-color: $bgCard;
            padding: 30px;
        }

        h5{
            font-weight: 100;
        }

        p{
            color: $textColor;
        }

        .ms_fs_icon{
            font-size: 60px;
            color: $colorButton;
            margin-bottom: 20px;
        }
    }

    .ms_bg{
        background-image: url('../assets/images/Untitled-1-1-1-1-1.png');
        padding: 110px;
    }
</style>