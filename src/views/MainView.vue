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
                <div class="ppp">
                    <div class="p_img"><img src="icon/teamB_icon.jpg"/></div>
                    <div class="p_sim">
                        <span>팀 프로젝트 : </span>
                        <h3>해양생물연구센터</h3>
                        <p>Html, Css, Scss, Javascript</p>
                        <div class="p_link">
                            <div class="icon" @click="ProjectLink('https://mingz-x.github.io/B/')"><img src="icon/teamB_icon_S.jpg"/></div>
                            <span/>
                            <div class="icon" @click="ProjectLink('https://github.com/mingz-x/B.git')"><img src="icon/github_icon.jpg"/></div>
                        </div>
                    </div>
                </div>
                <div class="p_deep">
                    <h2 class="project_in">프로젝트 소개 &#58; </h2>
                        <p>사이트 리뉴얼 작업으로 사용자의 편의성을 높이기 위해 ux/ui를 수정하고 반응형으로 제작하여 어떤 기기로 사이트에 방문하여도 이용에 불편함이 없도록 작업했습니다.</p> <br/>
                        <p>프로젝트는 html, css, scss, javascript를 이용하여 작업하였습니다.</p> <br/>
                    <h2>페이지 소개 &#58; </h2>
                        <p>‘인사말, 오시는 길, 구조ㆍ치료 활동, 서식지 외 보존 기관’ 페이지 제작을 맡았습니다.</p>
                </div>
            </div>
            <div class="p_contant">
                <div class="ppp">
                    <div class="p_img"><img src="icon/sema_icon.jpg"/></div>
                    <div class="p_sim">
                        <span>프로젝트 : </span>
                        <h3>Sema 서울시립미술관</h3>
                        <p>Html, Css, Javascript, Next.js, Nextauth, Firebase</p>
                        <div class="p_link">
                            <div class="icon" @click="ProjectLink('https://sema.vercel.app/')"><img src="icon/sema_icon_S.jpg"/></div>
                            <span/>
                            <div class="icon" @click="ProjectLink('https://github.com/mingz-x/sema.git')"><img src="icon/github_icon.jpg"/></div>
                        </div>
                    </div>
                </div>
                <div class="p_deep">
                    <h2 class="project_in">프로젝트 소개 : </h2>
                        <p>서울열린데이터광장에서 제공하는 서울시 오픈 API 중 관심가는 데이터인 미술관 데이터를 선택하여 기획했습니다.</p> <br/>
                        <p>프로젝트는 자바스크립트 프레임워크인 next.js를 사용하여 작업했습니다.</p> <br/>
                    <h2>페이지 소개 : </h2>
                        <p>모바일 앱으로 제작하여 큰 메뉴로는 ‘검색, 메뉴, 홈(메인), 스크랩, 마이페이지’로 크게 5개의 메뉴로 구성했습니다.</p>
                </div>
            </div>
            <div class="p_contant">
                <div class="ppp">
                    <div class="p_img"><img src="icon/movie_icon.jpg"/></div>
                    <div class="p_sim">
                        <span>프로젝트 : </span>
                        <h3>Movie</h3>
                        <p>Html, Css, Javascript, React.js</p>
                        <div class="p_link">
                            <div class="icon" @click="ProjectLink('https://movie-theta-black.vercel.app/')"><img src="icon/movie_icon_S.jpg"/></div>
                            <span/>
                            <div class="icon" @click="ProjectLink('https://github.com/mingz-x/movie.git')"><img src="icon/github_icon.jpg"/></div>
                        </div>
                    </div>
                </div>
                <div class="p_deep">
                    <h2 class="project_in">프로젝트 소개 : </h2>
                        <p>영화 오픈 API를 이용하여 영화 사이트를 기획했습니다.</p> <br/>
                        <!-- 영화 오픈 API를 이용하여 사이트를 제작했습니다. -->
                        <p>프로젝트는 자바스크립트 라이브러리인 react.js를 사용하여 작업했습니다.</p> <br/>
                        <!-- 프로젝트는 자바스크립트 라이브러리인 react.js를 사용하여 작업했습니다. -->
                    <h2>페이지 소개 : </h2>
                        <p>‘메인, 영화, 티비시리즈’ 3개의 메뉴와 상세페이지로 총 4개의 페이지로 제작했습니다.</p>
                        <!-- ‘메인, 영화, 티비시리즈’ 3개의 페이지와 상세페이지로 총 4개의 페이지로 제작했습니다. -->
                </div>
            </div>
            <div class="p_contant">
                <div class="ppp">
                    <div class="p_img"><img src="icon/news_icon.jpg"/></div>
                    <div class="p_sim">
                        <span>프로젝트 : </span>
                        <h3>News</h3>
                        <p>Html, Css, Javascript, Vue.js</p>
                        <div class="p_link">
                            <div class="icon" @click="ProjectLink('https://news-sable-one.vercel.app/')"><img src="icon/news_icon_S.jpg"/></div>
                            <span/>
                            <div class="icon" @click="ProjectLink('https://github.com/mingz-x/news.git')"><img src="icon/github_icon.jpg"/></div>
                        </div>
                    </div>
                </div>
                <div class="p_deep">
                    <h2 class="project_in">프로젝트 소개 : </h2>
                        <p>뉴스 오픈 API를 이용해서 뉴스 페이지를 기획했습니다.</p> <br/>
                        <p>프로젝트는 프로그레시브 자바스크립트 프레임워크인 vue.js를 사용하여 개발했습니다.</p> <br/>
                    <h2>페이지 소개/설명 : </h2>
                        <p>‘국내,해외’ 2개의 페이지 안에 ‘전체, 정치, 경제, 사회, 문화, 세계, 기술/IT, 연예, 사설’로 나누어 탭버튼을 개발하여 원하는 주제의 기사만 볼 수 있도록 기획하였습니다.</p>
                </div>
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
                        <div class="S_img"><img src="about/green_S.jpg"/></div>
                        <span>긍정적</span>
                    </div>
                    <div :class="['btn',{active:realIndex==1}]" @click="slideTo(1)">
                        <div class="S_img"><img src="about/red_S.jpg"/></div>
                        <span>분석적</span>
                    </div>
                    <div :class="['btn',{active:realIndex==2}]" @click="slideTo(2)">
                        <div class="S_img"><img src="about/yellow_S.jpg"/></div>
                        <span>창의적</span>
                    </div>
                    <div :class="['btn',{active:realIndex==3}]" @click="slideTo(3)">
                        <div class="S_img"><img src="about/blue_S.jpg"/></div>
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
                                <div class="B_img"><img src="about/green_B.jpg"/></div>
                                <div class="kw">
                                    <span># 긍정적인</span>
                                    <p>긍정적인 성격으로 문제 해결과 협업 등 팀워크에서 긍정적인 에너지를 발산합니다.</p>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="word">
                                <div class="B_img"><img src="about/red_B.jpg"/></div>
                                <div class="kw">
                                    <span># 분석적인</span>
                                    <p>차분하게 데이터를 분석하고 꼼꼼하게 작업하여 코드의 품질을 높입니다.</p>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="word">
                                <div class="B_img"><img src="about/yellow_B.jpg"/></div>
                                <div class="kw">
                                    <span># 창의적인</span>
                                    <p>창의적 사고로 혁신적인 해결책을 제시합니다.</p>
                                </div>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="word">
                                <div class="B_img"><img src="about/blue_B.jpg"/></div>
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
            <!-- <div class="conta">
                <div class="conta_img e-mail" ><img src="email_icon.svg"/></div>
                <p>email@email.com</p>
                <div class="conta_img"><img src="github_icon.svg"/></div>
                <p>github.com/github/Repository</p>
            </div> -->
            <div class="conta">
                <div>
                    <div class="conta_img"><img src="contact/email_icon.svg"/></div>
                    <p>email@email.com</p>
                </div>
                <div>
                    <div class="conta_img"><img src="contact/github_icon.svg"/></div>
                    <p>github.com/github/Repository</p>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/pagination';
import { Mousewheel, Pagination } from 'swiper/modules';
import { ref } from 'vue';

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
            contact : "contact"
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
                } 
                .default{
                    cursor: default;
                }
            }
        }
        h1{
            font-size: 6.25em; /* 100px */
            cursor: default;
        }
        .project{
            margin: 300px 0;
            .p_contant{
                // margin: 150px 300px;
                margin: 150px 120px;
                display: flex;
                align-items: flex-start;
                justify-content: center;
                // gap: 70px;
                .ppp{
                    // margin: 30px 0;
                    // margin-right: 70px;
                    border-right: 1px solid #eee;
                    padding: 30px 0;
                    padding-right: 70px;
                    .p_img{
                        width: 470px;
                        img{width: 100%;}
                    }
                    .p_sim{
                        text-align: left;
                        width: 470px;
                        margin-top: 20px;
                        span{
                            font-size: 1.5em; /* 24px */
                        }
                        h3{
                            font-size: 2.5em; /* 40px */
                            margin: 0;
                            margin-bottom: 20px;
                        }
                        p{
                            font-size: 1.875em; /* 30px */
                            margin: 0;
                        }
                        .p_link{
                            display: flex;
                            align-items: center;
                            justify-content: flex-start;
                            margin-top: 20px;
                            // .p_icon{
                            //     margin-right: 30px;
                            // }
                            // .g_icon{
                            //     margin-left: 30px;
                            // }
                            .icon{
                                cursor: pointer;
                            }
                            span{
                                border: 1px solid black;
                                height: 40px;
                                margin: 0 30px;
                            }
                        }
                    }
                }
                // .p_line{
                //     border: 1px solid #eee;
                //     height: 888px;
                // }
                .p_deep{
                    margin: 30px 0;
                    // padding: 30px 0;
                    text-align: left;
                    width: 610px;
                    // border-left: 1px solid #eee;
                    // padding-left: 70px;
                    margin-left: 70px;
                    .project_in{
                        margin-top: 0;
                    }
                    p{
                        font-size: 1.75em; /* 28px */
                        // margin: 20px 0;
                        margin: 0;
                    }
                }
            }
        }
        .about{
            margin: 300px 0;
            height: 100vh;
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
            h1{
                margin-bottom: 100px;
            }
            // .conta{
            //     display: flex;
            //     align-items: center;
            //     justify-content: center;
            //     gap: 40px;
            //     .conta_img{
            //         width: 80px;
            //         img{width: 100%;}
            //     }
            //     .e-mail{
            //         padding-right: 40px;
            //         border-right: 2px solid black;
            //     }
            // }
            .conta{
                div{
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    gap: 20px;
                    .conta_img{
                        width: 40px;
                        img{width: 100%;}
                    }
                    p{
                        font-size: 1.875em; /* 30px */
                        margin: 20px 0;
                    }
                }
            }
        }
    }
</style>