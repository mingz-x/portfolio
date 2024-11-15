<template lang="">
    <div class="main">
        <div class="intro">
            <h4>Park Minji</h4>
            <h1>Portfolio</h1>
            <div class="round">
                <p>
                    <span @click="point(project)">Project</span>
                    <span @click="point(about)">About</span>
                    <span @click="point(contact)">Contact</span>
                </p>
                <p>
                    <span>Frontend</span>
                    <span>Developer</span>
                </p>
            </div>
        </div>
        <div class="project" id="project">
            <h1>Project</h1>
            <!-- <div class="p_contant">
                <div class="ppp">
                    <div class="p_img"><img src="_icon.jpg"/></div>
                    <div class="p_sim">
                        <h4>프로젝트 이름</h4>
                        <p>간단 소개</p>
                        <p>주 사용 스택</p>
                        <p>배포 주소</p>
                        <p>깃허브 주소</p>
                    </div>
                </div>
                <div class="p_deep">
                    <p>프로젝트 소개/설명</p>
                    <p>담당파트</p>
                    <p>기능 소개/설명 (트러블슈팅)</p>
                    <p>구체적 스택/훅 사용 설명</p>
                </div>
            </div> -->
            <div class="p_contant">
                <div class="ppp">
                    <div class="p_img"><img src="teamB_icon.jpg"/></div>
                    <div class="p_sim">
                        <span>팀 프로젝트 : </span>
                        <h3>해양생물연구센터</h3>
                        <p>Html, Css, Scss, Javascript</p>
                        <p>배포 주소</p>
                        <p>깃허브 주소</p>
                    </div>
                </div>
                <!-- <div class="p_line"></div> -->
                <div class="p_deep">
                    <p>프로젝트 소개/설명</p>
                    <p>담당파트</p>
                    <p>기능 소개/설명</p>
                    <!-- <p>구체적 스택/훅 사용 설명</p> -->
                </div>
            </div>
            <div class="p_contant">
                <div class="ppp">
                    <div class="p_img"><img src="sema_icon.jpg"/></div>
                    <div class="p_sim">
                        <span>프로젝트 : </span>
                        <h3>Sema 서울시립미술관</h3>
                        <p>Html, Css, Javascript, Next.js, Nextauth, Firebase</p>
                        <p>배포 주소</p>
                        <p>깃허브 주소</p>
                    </div>
                </div>
                <div class="p_deep">
                    <p>프로젝트 소개/설명</p>
                    <p>담당파트</p>
                    <p>기능 소개/설명</p>
                    <!-- <p>구체적 스택/훅 사용 설명</p> -->
                </div>
            </div>
            <div class="p_contant">
                <div class="ppp">
                    <div class="p_img"><img src="movie_icon.jpg"/></div>
                    <div class="p_sim">
                        <span>프로젝트 : </span>
                        <h3>Movie</h3>
                        <p>Html, Css, Javascript, React.js</p>
                        <p>배포 주소</p>
                        <p>깃허브 주소</p>
                    </div>
                </div>
                <div class="p_deep">
                    <p>프로젝트 소개/설명</p>
                    <p>담당파트</p>
                    <p>기능 소개/설명</p>
                    <!-- <p>구체적 스택/훅 사용 설명</p> -->
                </div>
            </div>
            <div class="p_contant">
                <div class="ppp">
                    <div class="p_img"><img src="news_icon.jpg"/></div>
                    <div class="p_sim">
                        <span>프로젝트 : </span>
                        <h3>News</h3>
                        <p>Html, Css, Javascript, Vue.js</p>
                        <p>배포 주소</p>
                        <p>깃허브 주소</p>
                    </div>
                </div>
                <div class="p_deep">
                    <p>프로젝트 소개/설명</p>
                    <p>담당파트</p>
                    <p>기능 소개/설명</p>
                    <!-- <p>구체적 스택/훅 사용 설명</p> -->
                </div>
            </div>
        </div>
        <div class="about" id="about">
            <h1>About</h1>
            <div class="introduce">
                <!-- <p>자기소개 한 문장</p> -->
            </div>
            <div class="key">
                <div class="key_btn">
                    <div class="btn">
                        <div class="S_img"><img src="green_S.jpg"/></div>
                        <span>긍정적</span>
                    </div>
                    <div class="btn">
                        <div class="S_img"><img src="red_S.jpg"/></div>
                        <span>분석적</span>
                    </div>
                    <div class="btn">
                        <div class="S_img"><img src="yellow_S.jpg"/></div>
                        <span>창의적</span>
                    </div>
                    <div class="btn">
                        <div class="S_img"><img src="blue_S.jpg"/></div>
                        <span>의사소통</span>
                    </div>
                </div>
                <div class="key_word">
                    <div class="word">
                        <div class="B_img"><img src="green_B.jpg"/></div>
                        <div class="kw">
                            <span># 긍정적인</span>
                            <p>긍정적인 성격으로 문제 해결과 협업 등 팀워크에서 긍정적인 에너지를 발산합니다.</p>
                        </div>
                    </div>
                    <div class="word">
                        <div class="B_img"><img src="red_B.jpg"/></div>
                        <div class="kw">
                            <span># 분석적인</span>
                            <p>차분하게 데이터를 분석하고 꼼꼼하게 작업하여 코드의 품질을 높입니다.</p>
                        </div>
                    </div>
                    <div class="word">
                        <div class="B_img"><img src="yellow_B.jpg"/></div>
                        <div class="kw">
                            <span># 창의적인</span>
                            <p>창의적 사고로 혁신적인 해결책을 제시합니다.</p>
                        </div>
                    </div>
                    <div class="word">
                        <div class="B_img"><img src="blue_B.jpg"/></div>
                        <div class="kw">
                            <span># 의사소통</span>
                            <p>다양한 팀원들과의 협업에서 효과적인 의사소통 능력을 구사합니다.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="contact" id="contact">
            <h1>Contact</h1>
            <div class="conta">
                <div>
                    <div class="conta_img"><img src="email_icon.svg"/></div>
                    <p>email@email.com</p>
                </div>
                <div>
                    <div class="conta_img"><img src="github_icon.svg"/></div>
                    <p>github.com/github/Repository</p>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            project : "project",
            about : "about",
            contact : "contact"
        }
    },
    methods: {
        point(id) {
            const pointnav = document.getElementById(id);
            if (pointnav) {
                pointnav.scrollIntoView({
                    behavior: 'smooth',
                    block: 'start',
                });
            }
        }
    }
}
</script>
<style lang="scss">
    .main{
        max-width: 1440px;
        margin: 0 auto;
        .intro{
            margin: 300px 0;
            // margin-top: 250px;
            // margin-bottom: 300px;
            h4{
                margin: 0;
                font-size: 5em;  /* 80px */
                /* 6.25em = 100px */
            }
            h1{
                margin: 0;
                margin-bottom: 20px;
                font-size: 12.5em;  /* 200px */
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
                        border: 1px solid black;
                        border-radius: 25px;
                        font-size: 1.875em; /* 30px */
                    }
                }
            }
        }
        h1{
            font-size: 6.25em; /* 100px */
        }
        .project{
            margin-top: 300px;
            .p_contant{
                // margin: 150px 300px;
                margin: 150px 120px;
                display: flex;
                align-items: flex-start;
                justify-content: center;
                // gap: 70px;
                .ppp{
                    margin: 30px 0;
                    margin-right: 70px;
                    .p_img{
                        width: 470px;
                        img{width: 100%;}
                    }
                    .p_sim{
                        text-align: left;
                        width: 470px;
                        span{
                            font-size: 1.5em; /* 24px */
                        }
                        h3{
                            font-size: 2.5em;
                            margin: 0;
                            margin-bottom: 40px;
                        }
                        p{
                            font-size: 1.875em; /* 30px */
                            margin: 0;
                        }
                    }
                }
                // .p_line{
                //     border: 1px solid #eee;
                //     height: 888px;
                // }
                .p_deep{
                    // margin: 30px 0;
                    padding: 30px 0;
                    text-align: left;
                    width: 610px;
                    border-left: 1px solid #eee;
                    padding-left: 70px;
                    p{
                        font-size: 1.5em; /* 24px */
                        // margin: 20px 0;
                        margin: 0;
                    }
                }
            }
        }
        .about{
            margin-top: 300px;
            .introduce{
                p{
                    margin-top: 100px;
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
                    .btn{
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
                    .word{
                        display: flex;
                        align-items: center;
                        justify-content: center;
                        gap: 50px;
                        // padding: 30px 0;
                        margin: 150px 0;
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
                                margin-top: 0;
                                font-size: 1.5em; /* 24px */
                            }
                        }
                    }
                }
            }
        }
        .contact{
            margin: 300px 0;
            h1{
                margin-bottom: 100px;
            }
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