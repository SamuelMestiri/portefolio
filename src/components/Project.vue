<template>
    <div class="col-lg-2 col-md-6 col-sm-6 project">
        <div class="container-fluid">
            <div class="row">
                <div class="img-container">
                    <img src="../assets/test-projet.jpg" alt="image du project" class="pres-img" data-toggle="modal" data-target="#exampleModal">
                </div>
                <!-- Modal -->
                <div class="modal fade" id="exampleModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
                    <div class="modal-dialog modal-lg" role="document">
                        <div class="modal-content">
<!--                            <div class="modal-header">-->
<!--                                <h5 class="modal-title" id="exampleModalLabel">Modal title</h5>-->
<!--                                <button type="button" class="close" data-dismiss="modal" aria-label="Close">-->
<!--                                    <span aria-hidden="true">&times;</span>-->
<!--                                </button>-->
<!--                            </div>-->
                            <div class="modal-body">
                                <div class="container-fluid">
                                    <div class="row mt-3 mb-3">
                                        <div class="col-xl-4 col-lg-5 col-md-6">
                                            <img :src="imgName" class="rounded mx-auto d-block" alt="test">
                                        </div>
                                        <div class="col-xl-8 col-lg-7 col-md-6">
                                            <h3 class="mb-4 ml-4">{{ title }}</h3>
                                            <p class="rounded mx-auto d-block">{{ description }} Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium animi corporis ducimus ea eveniet fuga illo maiores maxime necessitatibus nobis, nulla numquam omnis pariatur perspiciatis placeat provident reiciendis repellat sequi!</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
<!--                            <div class="modal-footer">-->
<!--                                <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>-->
<!--                                <button type="button" class="btn btn-primary">Save changes</button>-->
<!--                            </div>-->
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Nav',
        props: {
            imgName: String,
            title: String,
            description: String,
        }
    }
</script>


<style lang="scss" scoped>
    .project{
        padding: 15px;
        .img-container{
            overflow: hidden;
            border: #000 1px solid;
        }
        .pres-img{
            width: 100%;
            height: 100%;
            transition: .5s ease-out;
            &:hover{
                cursor: pointer   ;
                -webkit-filter: brightness(60%); /* Safari 6.0 - 9.0 */
                filter: brightness(60%);
                transform: scale(1.1);
            }
        }
        .modal {
            .modal-dialog{
                margin: 0;
                margin-left: 15%;
                max-width: 70%;
                .modal-content {
                    margin-top: 250px;
                    background-color: #363636;
                    line-height: 26px;
                    .modal-body {
                        color: #FFF;
                        font-weight: 300;
                        img {
                            width: 80%;
                        }
                    }
                }
            }

        }
    }
</style>
