<template lang="">
    <div class="main">
        <div class="intro">
            <h4>Park Minji</h4>
            <h1>Portfolio</h1>
            <div class="round">
                <p class="pointer">
                    <span @click="point(project)">Project</span>
                    <span @click="point(about)">About</span>
                    <span @click="point(contact)">Contact</span>
                </p>
                <p class="default">
                    <span>Frontend</span>
                    <span>Developer</span>
                </p>
            </div>
        </div>
        <div class="project" id="project">
            <h1>Project</h1>
            <div class="p_contant">
                <Swiper
                    :modules="modules"
                    :slides-per-view="'auto'"
                    :direction="'horizontal'"
                    :space-between="20"
                    :scrollbar="{ el: '.swiper-scrollbar', draggable: true }"
                    :mousewheel="{ forceToAxis: true }"
                    class="custom-swiper"
                >
                    <SwiperSlide
                        v-for="(project, index) in projects" 
                        :key="index" 
                        @mouseover="hoverState[index] = true"
                        @mouseleave="hoverState[index] = false"
                    >
                        <div class="p_card">
                            <div class="card">
                                <div v-if="!hoverState[index]" class="card_img">
                                    <img :src="project.image" alt="Project image"/>
                                </div>
                                <div v-if="hoverState[index]" class="card_contant"
                                    @mouseover="isHovered = true" 
                                    @mouseleave="isHovered = false"
                                >
                                    <h3>{{ project.name }}</h3>
                                    <p>{{ project.description }}</p>
                                    <p>{{ project.technologies }}</p>
                                    <div class="c_icon">
                                        <div class="p_icon" @click="ProjectLink(project.projectLink)"><img :src="project.projectIcon" alt="Project icon"/></div>
                                        <span/>
                                        <div class="g_icon" @click="ProjectLink(project.githubLink)"><img :src="project.githubIcon" alt="GitHub icon"/></div>
                                    </div>
                                </div>
                            </div>
                            <h3 class="card_name">{{ project.name }}</h3>
                        </div>
                    </SwiperSlide>
                    <div class="swiper-scrollbar"></div>
                </Swiper>
            </div>
        </div>
        <div class="about" id="about">
            <h1>About</h1>
            <div class="introduce">
                <p>
                    어떤 문제라도 열린 마음으로 접근하고, 다양한 아이디어를 바탕으로 <br/> 효율적으로 해결책을 모색하며, 팀과 함께 나아갑니다.
                </p>
            </div>
            <div class="key">
                <div class="key_btn">
                    <div :class="['btn',{active:realIndex==0}]" @click="slideTo(0)">
                        <div class="S_img"><img src="about/positive_S.svg"/></div>
                        <span>긍정적</span>
                    </div>
                    <div :class="['btn',{active:realIndex==1}]" @click="slideTo(1)">
                        <div class="S_img"><img src="about/analytical_S.svg"/></div>
                        <span>분석적</span>
                    </div>
                    <div :class="['btn',{active:realIndex==2}]" @click="slideTo(2)">
                        <div class="S_img"><img src="about/creative_S.svg"/></div>
                        <span>창의적</span>
                    </div>
                    <div :class="['btn',{active:realIndex==3}]" @click="slideTo(3)">
                        <div class="S_img"><img src="about/communication_S.svg"/></div>
                        <span>의사소통</span>
                    </div>
                </div>
                <div class="key_word">
                        <swiper
                            @swiper="setSwiperRef"  
                            :direction="'vertical'"
                            :slidesPerView="3"
                            :spaceBetween="100"
                            :mousewheel="true"
                            :centeredSlides="true"
                            :modules="modules"
                            class="mySwiper"
                            @slideChange="onSlideChange"
                        >
                        <swiper-slide>
                            <div class="word">
                                <div class="B_img"><img src="about/positive_B.svg"/></div>
                                <div class="kw">
                                    <span># 긍정적인</span>
                                    <p>긍정적인 성격으로 문제 해결과 협업 등 팀워크에서 긍정적인 에너지를 발산합니다.</p>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="word">
                                <div class="B_img"><img src="about/analytical_B.svg"/></div>
                                <div class="kw">
                                    <span># 분석적인</span>
                                    <p>차분하게 데이터를 분석하고 꼼꼼하게 작업하여 코드의 품질을 높입니다.</p>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="word">
                                <div class="B_img"><img src="about/creative_B.svg"/></div>
                                <div class="kw">
                                    <span># 창의적인</span>
                                    <p>창의적 사고로 혁신적인 해결책을 제시합니다.</p>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="word">
                                <div class="B_img"><img src="about/communication_B.svg"/></div>
                                <div class="kw">
                                    <span># 의사소통</span>
                                    <p>다양한 팀원들과의 협업에서 효과적인 의사소통 능력을 구사합니다.</p>
                                </div>
                            </div>
                        </swiper-slide>
                    </swiper>
                </div>
            </div>
        </div>
        <div class="contact" id="contact">
            <h1>Contact</h1>
            <div class="conta">
                <div>
                    <div class="conta_img"><img src="contact/email_B.icon.svg"/></div>
                    <h3>email@email.com</h3>
                </div>
                <span/>
                <div>
                    <div class="conta_img"><img src="contact/github_B.icon.svg"/></div>
                    <h3>github.com/github</h3>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/pagination';
import { Mousewheel, Pagination, Scrollbar } from 'swiper/modules';
import { ref, onMounted } from 'vue';

const modules = [Mousewheel, Scrollbar];
const hoverState = ref([]);
const isHovered = ref(false);


export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
        // Create array with 500 slides
      const slides = ref(
        Array.from({ length: 4 }).map((_, index) => `Slide ${index + 1}`)
      );
      let swiperRef = null;
      let realIndex = ref(0);

      const setSwiperRef = (swiper) => {
        swiperRef = swiper;
      };
      const slideTo = (index) => {
        realIndex.value = index;
        swiperRef.slideTo(index);
      };

      function onSlideChange(e) {
        realIndex.value = e.activeIndex;        
      }
      
      return {
        slides,
        swiperRef: null,
        setSwiperRef,
        slideTo,
        realIndex,   
        onSlideChange,     
        modules: [Pagination, Mousewheel],
      };
      
    },
    
    data() {
        return {
            project : "project",
            about : "about",
            contact : "contact",
            
            // isHovered: false,
            hoverState: Array(4).fill(false),
            projects : [
                {
                    name: "해양생물연구센터",
                    description: "팀프로젝트 작업 \n 노후화 된 사이트 리뉴얼 \n 인사말, 오시는 길, 구조, 보호 페이지 제작",
                    technologies: "html, css, scss, javascript",
                    image: "project/teamB_B.icon.svg",
                    projectIcon: "project/teamB_S.icon.svg",
                    githubIcon: "project/github_S.icon.svg",
                    projectLink: "",
                    githubLink: "",
                    isHovered: false
                },
                {
                    name: "Sema 서울시립미술관",
                    description: "서울열린데이터광장 제공 \n 서울시 오픈 API 사용",
                    technologies: "Html, Css, Javscript, \n Next.js, Firebase, Nextauth",
                    image: "project/sema_B.icon.svg",
                    projectIcon: "project/sema_S.icon.svg",
                    githubIcon: "project/github_S.icon.svg",
                    projectLink: "",
                    githubLink: "",
                    isHovered: false
                },
                {
                    name: "Movie",
                    description: "영화 오픈 API 사용",
                    technologies: "Html, Css, Javscript, React.js",
                    image: "project/movie_B.icon.svg",
                    projectIcon: "project/movie_S.icon.svg",
                    githubIcon: "project/github_S.icon.svg",
                    projectLink: "",
                    githubLink: "",
                    isHovered: false
                },
                {
                    name: "News",
                    description: "뉴스 오픈 API 사용",
                    technologies: "Html, Css, Javscript, Vue.js",
                    image: "project/news_B.icon.svg",
                    projectIcon: "project/news_S.icon.svg",
                    githubIcon: "project/github_S.icon.svg",
                    projectLink: "",
                    githubLink: "",
                    isHovered: false
                },
            ]
        }
    },
    methods: {
        // handleClick(url, id) {
        //     this.ProjectLink(url);
        //     this.point(id);
        // }, /* 선택사항(코드를 깔끔하게 유지하고 재사용성을 높이는 방법) */
        point(id) {
            const pointnav = document.getElementById(id);
            if (pointnav) {
                pointnav.scrollIntoView({
                    behavior: 'smooth',
                    block: 'start',
                });
            }
        },
        
        ProjectLink(url){
            window.open(url, '_blank');
        }
    },
    mounted() {
        // nextTick(() => {
        // const swiperEl = document.querySelector(".custom-swiper").swiper;
        // const thumbEl = document.querySelector(".custom-scrollbar-thumb");

        // swiperEl.on("scroll", () => {
        //     const progress = swiperEl.getTranslate() / swiperEl.maxTranslate();
        //     thumbEl.style.transform = `translateX(${progress * 70}%)`;
        // });
        // });

        onMounted(() => {
            // Swiper 인스턴스가 정상적으로 동작하도록 설정
            const swiper = new Swiper('.custom-swiper', {
                modules: [Mousewheel, Scrollbar],
                slidesPerView: 'auto',
                direction: 'horizontal',  // 가로로 스크롤
                spaceBetween: 20,         // 슬라이드 간격
                mousewheel: {
                forceToAxis: true,      // 마우스휠로 가로 스크롤
                },
                scrollbar: {
                draggable: true,        // 스크롤바 드래그 가능
                },
            });
        });
        
    }, 
}
</script>
<style lang="scss">
    .main{
        max-width: 1440px;
        margin: 0 auto;
        img{vertical-align: middle;}
        .intro{
            height: 100vh;
            align-content: center;
            h4{
                margin: 0;
                font-size: 5em;  /* 80px */
                /* 6.25em = 100px */
                cursor: default;
            }
            h1{
                margin: 0;
                margin-bottom: 20px;
                font-size: 12.5em;  /* 200px */
                cursor: default;
            }
            .round{
                p{
                    margin: 10px 0;
                    span{
                        display: inline-block;
                        width: 264px;
                        margin: 5px 10px;
                        padding: 7px 20px;
                        text-align: center;
                        border: 2px solid black;
                        border-radius: 25px;
                        font-size: 1.875em; /* 30px */
                    }
                }
                .pointer{
                    span{
                        cursor: pointer;
                    }
                    span:hover{
                        background-color: black;
                        color: white;
                    } 
                }
                .default{
                    cursor: default;
                }
            }
        }
        h1{
            font-size: 6.25em; /* 100px */
            cursor: default;
            margin-bottom: 150px;
        }
        .project{
            height: 100vh;
            
            /* Swiper 컨테이너에 가로 스크롤 추가 */
            .swiper-container {
                width: 100%;  /* 🔹 컨테이너의 너비 100%로 설정 */
                height: 600px; /* 🔹 컨테이너의 고정 높이 설정 */
                overflow: hidden;  /* 🔹 넘치는 컨텐츠는 숨김 */
            }
            /* 기본 Swiper 스크롤바 */
            .swiper-scrollbar {
                // background: rgba(0, 0, 0, 0.1);
                // height: 8px;  /* 🔹 스크롤바 높이 설정 */
                // border-radius: 4px;
                position: absolute;
                bottom: 10px;  /* ✅ 스크롤바 위치 조정 */
                left: 50%;
                transform: translateX(-50%);
                width: 80%;  /* ✅ 스크롤바 너비 조정 */
                height: 8px;  /* ✅ 스크롤바 높이 */
                background: rgba(0, 0, 0, 0.1);
                border-radius: 4px;
            }
            .swiper-scrollbar-drag {
                background: #007aff; /* 🔹 스크롤바 색상 설정 */
                border-radius: 4px;
            }
            .swiper-slide{
                width: fit-content;
            }
            
            margin: 300px 0;
            .p_contant{
                margin: 150px 100px;
                display: flex;
                flex-direction: row;
                flex-wrap: nowrap;
                gap: 20px;
                justify-content: flex-start;
                .p_card{
                    // width: fit-content;
                    border: 1px solid black;
                    width: 400px;
                    height: 600px;
                }
                .card{
                    // border: 1px solid black;
                    // width: 400px;
                    // height: 500px;
                    .card_img{
                        padding: 140px 90px;
                        width: 220px;
                        img{width: 100%;}
                    }
                    .card_contant{
                        padding: 50px 40px;
                        width: 320px;
                        height: 400px;
                        h3{
                            font-size: 30px;
                            border-bottom: 2px solid black;
                            margin: 0;
                            padding-bottom: 30px;
                            margin-bottom: 50px;
                        }
                        p{
                            font-size: 25px;
                        }
                        .c_icon{
                            display: flex;
                            justify-content: center;
                            align-items: center;
                            gap: 30px;
                            .p_icon{
                                width: 60px;
                                img{width: 100%;}
                            }
                            span{
                                border: 1px solid black;
                                height: 37px;
                            }
                            .g_icon{
                                width: 55px;
                                img{width: 100%;}
                            }
                        }
                    }
                }
                .card_name{
                    // width: 400px;
                    // border: 1px solid black;
                    background-color: black;
                    color: white;
                    font-size: 30px;
                    // font-weight: bold;
                    padding: 30px 0;
                    margin: 0;
                }
            }
        }
        .about{
            margin: 300px 0;
            // height: 100vh;
            .introduce{
                p{
                    // margin-top: 100px;
                    margin: 100px 120px;
                    // margin-bottom: 50px;
                    font-size: 1.875em; /* 30px */
                }
            }
            .key{
                display: flex;
                align-items: center;
                // justify-content: center;
                // gap: 250px;
                justify-content: space-around;
                // justify-content: space-evenly;
                .key_btn{
                    .btn.active{
                        opacity: 1;
                    }
                    .btn{
                        opacity: 0.2;
                        display: flex;
                        align-items: center;
                        justify-content: space-between;
                        gap: 20px;
                        // padding: 10px 0;
                        // margin: 50px;
                        margin: 20px;
                        .S_img{
                            width: 30px;
                            img{width: 100%;}
                        }
                        span{
                            width: 100px;
                            text-align: left;
                            font-weight: 500;
                            // font-size: 1.25em; /* 20px */
                            font-size: 1.5em; /* 24px */
                            color: #333;
                        }
                    }
                }
                .key_word{
                    height: 600px;
                    .swiper{
                        height: 100%;
                    }
                    .swiper-slide{
                        opacity: 0.2;
                    }
                    .swiper-slide-active{
                        opacity: 1;
                    }
                    .word{
                        display: flex;
                        align-items: center;
                        justify-content: center;
                        gap: 50px;
                        // padding: 30px 0;
                        .B_img{
                            width: 100px;
                            img{width: 100%;}
                        }
                        .kw{
                            width: 340px;
                            text-align: left;
                            span{
                                color: #555;
                                font-weight: bold;
                                font-size: 1.5em; /* 24px */
                            }
                            p{
                                // margin-top: 0;
                                margin: 0;
                                font-size: 1.5em; /* 24px */
                            }
                        }
                    }
                }
            }
        }
        .contact{
            height: 100vh;
            align-content: center;
            .conta{
                display: flex;
                align-items: center;
                justify-content: center;
                gap: 100px;
                div{
                    display: inline-block;
                    .conta_img{
                        width: 100px;
                        img{width: 100%;}
                    }
                    h3{
                        font-size: 30px;
                    }
                }
                span{
                    border: 1px solid black;
                    height: 150px;
                }
            }
        }
    }
</style>