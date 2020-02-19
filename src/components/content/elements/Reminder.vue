<template>
    <div class="reminder">
                <h2 class="r-title">Mener vos entretiens à la perfection</h2>
                <div class="reminder-content">
                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="30.849" height="30.849" viewBox="0 0 30.849 30.849">
                                <path id="Icon_metro-warning" data-name="Icon metro-warning" d="M17.995,4.723,30.922,30.487H5.068L17.995,4.723Zm0-2.795a2.23,2.23,0,0,0-1.834,1.345L2.994,29.516c-1.009,1.793-.151,3.261,1.907,3.261H31.089c2.058,0,2.916-1.467,1.907-3.261h0L19.829,3.273a2.23,2.23,0,0,0-1.834-1.345Zm1.928,25.064a1.928,1.928,0,1,1-1.928-1.928A1.928,1.928,0,0,1,19.923,26.992Zm-1.928-3.856a1.928,1.928,0,0,1-1.928-1.928V15.424a1.928,1.928,0,1,1,3.856,0v5.784A1.928,1.928,0,0,1,17.995,23.136Z" transform="translate(-2.571 -1.928)" fill="#fff"/>
                            </svg>
                            <p>Informez le participant de la raison de l’entretien avant de le commencer</p>
                        </div>
                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="33" viewBox="0 0 24 33">
                                <path id="Icon_material-loop" data-name="Icon material-loop" d="M18,6V1.5l-6,6,6,6V9a9.007,9.007,0,0,1,9,9,8.806,8.806,0,0,1-1.05,4.2l2.19,2.19A11.979,11.979,0,0,0,18,6Zm0,21a9.007,9.007,0,0,1-9-9,8.806,8.806,0,0,1,1.05-4.2L7.86,11.61A11.979,11.979,0,0,0,18,30v4.5l6-6-6-6Z" transform="translate(-6 -1.5)" fill="#fff"/>
                            </svg>
                            <p>Laissez le parler !</p>
                        </div>

                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="33" height="33" viewBox="0 0 33 33">
                                <g id="Icon_feather-info" data-name="Icon feather-info" transform="translate(-1.5 -1.5)">
                                    <path id="Tracé_173" data-name="Tracé 173" d="M33,18A15,15,0,1,1,18,3,15,15,0,0,1,33,18Z" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                    <path id="Tracé_174" data-name="Tracé 174" d="M18,24V18" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                    <path id="Tracé_175" data-name="Tracé 175" d="M18,12h0" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                </g>
                            </svg>
                            <p>Ne l’influencez pas pour qu’il réponde à vos attentes personnelles.</p>
                        </div>

                        <div class="inter-box">
                            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 30 30">
                                <path id="Icon_feather-message-circle" data-name="Icon feather-message-circle" d="M31.5,17.25a12.57,12.57,0,0,1-1.35,5.7A12.75,12.75,0,0,1,18.75,30a12.57,12.57,0,0,1-5.7-1.35L4.5,31.5l2.85-8.55A12.57,12.57,0,0,1,6,17.25a12.75,12.75,0,0,1,7.05-11.4,12.57,12.57,0,0,1,5.7-1.35h.75a12.72,12.72,0,0,1,12,12Z" transform="translate(-3 -3)" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                            </svg>
                            <p>Réaliser une dizaine d'entretiens.</p>
                        </div>
                </div>
    </div>
</template>

<script>
export default {
    
}
</script>


<style lang="scss">
    .reminder {
        background-color: #3F3D56;
        font-family: "Montserrat", sans-serif;
        font-size: 1em;
        padding: 10px 20px;
        margin: 40px 0;
        text-align: left;

        .r-title {
            color: white;
            text-align: center;
            font-weight: 700;
            font-size: 1.2em;
            padding: 10px 0;
        }

        .reminder-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            grid-template-rows: 1fr 1fr;
            grid-row-gap: 1rem;
            grid-column-gap: 1rem;
            font-weight: 400;
            padding: 10px;

            .inter-box {
                display: flex;
                align-items: center;

                p {
                    margin: 0 20px;
                    color: white;
                }
            }
        }
    }
</style>