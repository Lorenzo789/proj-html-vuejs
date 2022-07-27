<template>
    <main class="container-fluid">

        <NavBarMain />

        <SectionInvestingMain v-for="(element, index) in  sectionInvesting" :key="index" :title="element.title"
            :subTitle="element.subTitle" />

        <div class="container p-2 my-5">
            <div class="row my-5">
                <div class="ms_card">
                    <i class="fa-solid fa-earth-europe ms_fs_icon"></i>
                    <h5>Worldwide Recognize</h5>
                    <p>Our online courses certificates can be used around the world and also in most popular
                        universities and companies
                    </p>
                </div>
                <div class="ms_card">
                    <i class="fa-solid fa-tv ms_fs_icon"></i>
                    <h5>Mostly online Learning (sd)</h5>
                    <p>Masterstudy online certificates can be obtained in a range of specialized areas and typically
                        take about a year to complete
                    </p>
                </div>
                <div class="ms_card">
                    <i class="fa-solid fa-calendar-check ms_fs_icon"></i>
                    <h5>Graduate in as little as 1 Year</h5>
                    <p>Online post graduate certificates are a popular way to develop your professional
                        qualifications of Masterstudy
                    </p>
                </div>
            </div>
        </div>

        <SectionListCoursesMain />

        <SectionLearningMain v-for="(element, index) in sectionLearning" :key="index"
            :title="element.title"
            :subTitle="element.subTitle"
            :imgBg="element.imgBg"
        />

        <div class="container p-2 my-5">
            <h1>Recent courses</h1>
            <!-- COMPONENT GENERE CORSI -->
            <div>
                <ul>
                    <li>a</li>
                    <li>b</li>
                    <li>c</li>
                    <li>d</li>
                    <li>e</li>
                    <li>f</li>
                    <li>g</li>
                </ul>
            </div>
            <!-- COMPONENT GENERE CORSI -->

            <!-- COMPONENT CARD CORSI -->
            <div>
                <div class="row">
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
                </div>

                <div class="row">
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
                </div>

                <!-- TENDINA LATERALE -->
                <div></div>
                <!-- TENDINA LATERALE -->

                <!-- COMPONENT BUTTON -->
                <button>JOIN</button>
                <!-- COMPONENT BUTTON -->
            </div>
            <!-- COMPONENT CARD CORSI -->
        </div>

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
                    imgBg: require('../assets/images/Untitled-1-1-1-1-1.png'),
                }
            ],
        };
    },
    components: { NavBarMain, SectionInvestingMain, SectionListCoursesMain, SectionLearningMain }
}
</script>

<style lang="scss" scoped>
@import'../styles/variables.scss';

    .ms_card{
        background-color: $bgCard;
        width: calc(100% / 3 - 25px);
        padding: 30px;
        margin-right: 25px;

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

</style>