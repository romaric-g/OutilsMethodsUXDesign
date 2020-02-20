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
                                <p>Recherche</p>
                            </div>
                            <div class="section-links">
                                <ul>
                                    <li><p>Entretiens</p></li>
                                    <li><p>Observation</p></li>
                                    <li><p>Focus group</p></li>
                                    <li><p>Persona</p></li>
                                    <li><p>Expérience Map</p></li>
                                    <li><p>Complétion des phrases</p></li>
                                    <li><p>Test de connaissance</p></li>
                                </ul>
                            </div>
                        </li>
                        <li>
                            <div class="section-title">
                                <div class="section-icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="27.466" height="25.144" viewBox="0 0 27.466 25.144">
                                    <defs>
                                        <clipPath id="clip-path">
                                        <rect width="27.466" height="25.144" fill="none"/>
                                        </clipPath>
                                    </defs>
                                    <g id="Grille_de_répétition_1" data-name="Grille de répétition 1" clip-path="url(#clip-path)">
                                        <g transform="translate(-713 -1046.97)">
                                        <path id="Icon_open-magnifying-glass" data-name="Icon open-magnifying-glass" d="M11.909-.014C5.342-.014,0,4.876,0,10.888s5.342,10.9,11.909,10.9a12.648,12.648,0,0,0,5.648-1.277,3.274,3.274,0,0,0,.442.4l3.4,3.115a3.673,3.673,0,0,0,3.426.974,3.337,3.337,0,0,0,2.537-2.322A3.015,3.015,0,0,0,26.3,19.547l-3.4-3.115a3.363,3.363,0,0,0-.544-.4,10.061,10.061,0,0,0,1.5-5.17c0-6.011-5.342-10.9-11.909-10.9Zm0,3.115c4.729,0,8.506,3.457,8.506,7.787a7.455,7.455,0,0,1-2.246,5.357l-.1.093a3.274,3.274,0,0,0-.442.4,8.983,8.983,0,0,1-5.75,1.962c-4.729,0-8.506-3.457-8.506-7.787s3.777-7.787,8.506-7.787Z" transform="translate(713 1047.015)" fill="#3f3d56"/>
                                        </g>
                                    </g>
                                    </svg>

                                </div>
                                <p>Analyse</p>
                            </div>
                            <div class="section-links">
                                <ul>
                                    <li><p>Brainstorming</p></li>
                                    <li><p>Carte d’idéation</p></li>
                                    <li><p>Focus group</p></li>
                                    <li><p>Persona</p></li>
                                    <li><p>Expérience Map</p></li>
                                    <li><p>Complétion des phrases</p></li>
                                    <li><p>Test de connaissance</p></li>
                                </ul>
                            </div>
                        </li>
                        <li>
                            <div class="section-title">
                                <div class="section-icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="23.097" height="24.164" viewBox="0 0 23.097 24.164">
                                    <path id="Icon_awesome-book" data-name="Icon awesome-book" d="M23.1,16.991V1.133A1.186,1.186,0,0,0,21.86,0H4.949A4.755,4.755,0,0,0,0,4.531v15.1a4.755,4.755,0,0,0,4.949,4.531H21.86A1.186,1.186,0,0,0,23.1,23.032v-.755a1.108,1.108,0,0,0-.459-.883,9.648,9.648,0,0,1,0-3.526A1.092,1.092,0,0,0,23.1,16.991ZM6.6,6.324a.3.3,0,0,1,.309-.283h10.93a.3.3,0,0,1,.309.283v.944a.3.3,0,0,1-.309.283H6.908A.3.3,0,0,1,6.6,7.268Zm0,3.021a.3.3,0,0,1,.309-.283h10.93a.3.3,0,0,1,.309.283v.944a.3.3,0,0,1-.309.283H6.908a.3.3,0,0,1-.309-.283Zm13.064,11.8H4.949a1.516,1.516,0,1,1,0-3.021H19.663A15.56,15.56,0,0,0,19.663,21.144Z" fill="#3f3d56"/>
                                    </svg>
                                </div>
                                <p>Création</p>
                            </div>
                            <div class="section-links">
                                <ul>
                                    <li><p>Brainstorming</p></li>
                                    <li><p>Carte d’idéation</p></li>
                                    <li><p>Focus group</p></li>
                                    <li><p>Persona</p></li>
                                    <li><p>Expérience Map</p></li>
                                    <li><p>Complétion des phrases</p></li>
                                    <li><p>Test de connaissance</p></li>
                                </ul>
                            </div>
                        </li>
                        <li>
                            <div class="section-title">
                                <div class="section-icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="26.777" height="20.938" viewBox="0 0 26.777 20.938">
                                    <path id="Icon_material-directions-bike" data-name="Icon material-directions-bike" d="M17.293,6.335a2.15,2.15,0,0,0,2.231-2.043,2.24,2.24,0,0,0-4.463,0A2.15,2.15,0,0,0,17.293,6.335ZM5.579,12.974A5.306,5.306,0,0,0,0,18.081a5.306,5.306,0,0,0,5.579,5.107,5.306,5.306,0,0,0,5.579-5.107A5.306,5.306,0,0,0,5.579,12.974Zm0,8.682a3.8,3.8,0,0,1-3.9-3.575,3.8,3.8,0,0,1,3.9-3.575,3.8,3.8,0,0,1,3.9,3.575A3.8,3.8,0,0,1,5.579,21.656ZM12.05,11.442l2.678-2.451.893.817a8.192,8.192,0,0,0,5.69,2.145V9.91a5.8,5.8,0,0,1-4.017-1.532l-2.12-1.941a2.888,2.888,0,0,0-1.785-.613,1.953,1.953,0,0,0-1.562.613L8.7,9.3a1.937,1.937,0,0,0-.669,1.43,1.653,1.653,0,0,0,.669,1.43l3.57,2.86v5.107H14.5V13.791ZM21.2,12.974a5.306,5.306,0,0,0-5.579,5.107A5.306,5.306,0,0,0,21.2,23.188a5.306,5.306,0,0,0,5.579-5.107A5.306,5.306,0,0,0,21.2,12.974Zm0,8.682a3.8,3.8,0,0,1-3.9-3.575,3.8,3.8,0,0,1,3.9-3.575,3.8,3.8,0,0,1,3.9,3.575A3.8,3.8,0,0,1,21.2,21.656Z" transform="translate(0 -2.25)" fill="#3f3d56"/>
                                    </svg>
                                </div>
                                <p>Tester</p>
                            </div>
                            <div class="section-links">
                                <ul>
                                    <li><p>Brainstorming </p></li>
                                    <li><p>Carte d’idéation</p></li>
                                    <li><p>Focus group</p></li>
                                    <li><p>Persona</p></li>
                                    <li><p>Expérience Map</p></li>
                                    <li><p>Complétion des phrases</p></li>
                                    <li><p>Test de connaissance</p></li>
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

@media screen and (max-width: 800px) {
    nav {
        
    }
}

</style>