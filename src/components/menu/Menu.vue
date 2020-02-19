<template>
    <nav :class="{close}">
        <div class="head">
            <div class="reduce" @click="toggleMenu">
                <div class="reduce-text"><div class="content"><p>Réduire le menu</p></div></div>
                <div class="reduce-icon"><svg xmlns="http://www.w3.org/2000/svg" width="13.503" height="23.619" viewBox="0 0 13.503 23.619"><path id="Icon_ionic-ios-arrow-up" data-name="Icon ionic-ios-arrow-up" d="M18,15.321l8.93,8.937a1.688,1.688,0,1,0,2.384-2.391L19.2,11.742a1.685,1.685,0,0,0-2.327-.049L6.68,21.86a1.688,1.688,0,0,0,2.384,2.391Z" transform="translate(-11.251 29.806) rotate(-90)"/></svg></div>
            </div>
        </div>
        <div class="content">
            <simplebar class="menu" data-simplebar-auto-hide="false">
                    <ul>
                        <li>
                            <div class="section-title">
                                <div class="section-icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="36.455" height="22.248" viewBox="0 0 36.455 22.248"><path id="Icon_awesome-eye" data-name="Icon awesome-eye" d="M36.235,14.778A20.55,20.55,0,0,0,18.228,4.5,20.553,20.553,0,0,0,.22,14.779a1.734,1.734,0,0,0,0,1.691A20.55,20.55,0,0,0,18.228,26.748,20.553,20.553,0,0,0,36.235,16.469,1.734,1.734,0,0,0,36.235,14.778ZM18.228,23.967c-5.033,0-9.114-3.735-9.114-8.343s4.08-8.343,9.114-8.343,9.114,3.735,9.114,8.343S23.262,23.969,18.228,23.967Zm0-13.905a6.55,6.55,0,0,0-1.6.22,2.6,2.6,0,0,1-.3,3.6,3.24,3.24,0,0,1-3.936.273,5.328,5.328,0,0,0,2.473,6.062,6.52,6.52,0,0,0,7.065-.2,5.279,5.279,0,0,0,2.05-6.193,6.047,6.047,0,0,0-5.753-3.761Z" transform="translate(0 -4.5)" fill="#3f3d56"/></svg>
                                </div>
                                <p>Titre de section</p>
                            </div>
                            <div class="section-links">
                                <ul>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                </ul>
                            </div>
                        </li>
                        <li>
                            <div class="section-title">
                                <div class="section-icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="36.455" height="22.248" viewBox="0 0 36.455 22.248"><path id="Icon_awesome-eye" data-name="Icon awesome-eye" d="M36.235,14.778A20.55,20.55,0,0,0,18.228,4.5,20.553,20.553,0,0,0,.22,14.779a1.734,1.734,0,0,0,0,1.691A20.55,20.55,0,0,0,18.228,26.748,20.553,20.553,0,0,0,36.235,16.469,1.734,1.734,0,0,0,36.235,14.778ZM18.228,23.967c-5.033,0-9.114-3.735-9.114-8.343s4.08-8.343,9.114-8.343,9.114,3.735,9.114,8.343S23.262,23.969,18.228,23.967Zm0-13.905a6.55,6.55,0,0,0-1.6.22,2.6,2.6,0,0,1-.3,3.6,3.24,3.24,0,0,1-3.936.273,5.328,5.328,0,0,0,2.473,6.062,6.52,6.52,0,0,0,7.065-.2,5.279,5.279,0,0,0,2.05-6.193,6.047,6.047,0,0,0-5.753-3.761Z" transform="translate(0 -4.5)" fill="#3f3d56"/></svg>
                                </div>
                                <p>Titre de section</p>
                            </div>
                            <div class="section-links">
                                <ul>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                </ul>
                            </div>
                        </li>
                        <li>
                            <div class="section-title">
                                <div class="section-icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="36.455" height="22.248" viewBox="0 0 36.455 22.248"><path id="Icon_awesome-eye" data-name="Icon awesome-eye" d="M36.235,14.778A20.55,20.55,0,0,0,18.228,4.5,20.553,20.553,0,0,0,.22,14.779a1.734,1.734,0,0,0,0,1.691A20.55,20.55,0,0,0,18.228,26.748,20.553,20.553,0,0,0,36.235,16.469,1.734,1.734,0,0,0,36.235,14.778ZM18.228,23.967c-5.033,0-9.114-3.735-9.114-8.343s4.08-8.343,9.114-8.343,9.114,3.735,9.114,8.343S23.262,23.969,18.228,23.967Zm0-13.905a6.55,6.55,0,0,0-1.6.22,2.6,2.6,0,0,1-.3,3.6,3.24,3.24,0,0,1-3.936.273,5.328,5.328,0,0,0,2.473,6.062,6.52,6.52,0,0,0,7.065-.2,5.279,5.279,0,0,0,2.05-6.193,6.047,6.047,0,0,0-5.753-3.761Z" transform="translate(0 -4.5)" fill="#3f3d56"/></svg>
                                </div>
                                <p>Titre de section</p>
                            </div>
                            <div class="section-links">
                                <ul>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                </ul>
                            </div>
                        </li>
                        <li>
                            <div class="section-title">
                                <div class="section-icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="36.455" height="22.248" viewBox="0 0 36.455 22.248"><path id="Icon_awesome-eye" data-name="Icon awesome-eye" d="M36.235,14.778A20.55,20.55,0,0,0,18.228,4.5,20.553,20.553,0,0,0,.22,14.779a1.734,1.734,0,0,0,0,1.691A20.55,20.55,0,0,0,18.228,26.748,20.553,20.553,0,0,0,36.235,16.469,1.734,1.734,0,0,0,36.235,14.778ZM18.228,23.967c-5.033,0-9.114-3.735-9.114-8.343s4.08-8.343,9.114-8.343,9.114,3.735,9.114,8.343S23.262,23.969,18.228,23.967Zm0-13.905a6.55,6.55,0,0,0-1.6.22,2.6,2.6,0,0,1-.3,3.6,3.24,3.24,0,0,1-3.936.273,5.328,5.328,0,0,0,2.473,6.062,6.52,6.52,0,0,0,7.065-.2,5.279,5.279,0,0,0,2.05-6.193,6.047,6.047,0,0,0-5.753-3.761Z" transform="translate(0 -4.5)" fill="#3f3d56"/></svg>
                                </div>
                                <p>Titre de section</p>
                            </div>
                            <div class="section-links">
                                <ul>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                    <li><p>Lien vers section</p></li>
                                </ul>
                            </div>
                        </li>                                     
                    </ul>
            </simplebar>
        </div>
    </nav>
</template>

<script>
import simplebar from 'simplebar-vue';
import 'simplebar/dist/simplebar.min.css';

export default {
    data() {
        return {
            close: false
        }
    },
    components: {
        simplebar
    },
    methods: {
        toggleMenu() {
            this.close = !this.close;
            console.log("tesr")
        }
    }
}
</script>

<style lang="scss">
nav {
    width: 360px;
    height: 100vh;
    background-color: white;
    box-shadow: 2px 0 10px black;
    display: flex;
    flex-direction: column;

    transition-duration: 0.4s;

    .head {
        position: relative;
        font-family: 'Lato', sans-serif;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        overflow: hidden;

        .reduce {
            padding: 20px;
            cursor: pointer;
        }

        .reduce-text {
            position: absolute;

            height: 100%;
            left: 300px;
            font-size: 1.1em;
            line-height: 1em;
            font-weight: 600;
            .content {
                position: absolute;
                width: 360px;
                text-align: right;
                right: 0;
                top: 0;
                bottom: 0;
                p {
                    line-height: 100%;
                }
            }
        }
        .reduce-icon {
            transition-duration: 0.2s;
            transition-duration: 0.2s;
            svg {
                height: 18px;
                margin-left: 10px;
            }
        }

    }
    .content {
        position: relative;
        flex: 1;
        p {
            white-space: nowrap;
        }
        .menu {
            position: absolute;
            top: 0;right: 0;left: 0;bottom: 0;
            padding-top: 40px;
            padding-left: 40px; 

            .section-title {
                text-transform: uppercase;
                position: relative;
                font-family: 'Lato', sans-serif;
                margin: 2px 0;
                display: flex;
                p {
                    font-size: 1.3em;
                    font-weight: 700;
                    line-height: 40px;
                }
                svg {
                    height: 40px;
                    width: 40px;
                    padding: 5px;
                }
            }

            ul {
                list-style-type: none;
                .section-links {
                    p {
                        line-height: 1.3em;
                        font-family: 'Lato', sans-serif;
                    }
                    ul {
                        margin-left: 40px;
                    }
                }  
            }   
        }
    }
}

nav.close {
    width: 65px;
    .section-links{
        display: none;
    }

    p {
        white-space: unset!important;
    }

    .reduce-icon {
        transform: rotate(180deg);
    }
    
    .content .section-title {
        flex-direction: column;
        margin: 15px 0;

        p {
            font-size: 10px!important;
            line-height: 14px;
            max-width: 65px;
            text-align: center;
            margin: 0 auto;
        }
    }
    .menu {
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 0;
        .simplebar-content {
            height: 100%;
            & > ul {
                height: 100%;
                display: flex;
                flex-direction: column;
                justify-content: center;
            }
        }
    }

    .section-icon {
        display: flex;
        svg {
            margin: 0 auto;
        }
    }
}


</style>