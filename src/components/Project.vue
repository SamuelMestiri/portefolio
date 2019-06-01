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
                                        <div class="col-3">
                                            <img src="../assets/test-projet.jpg" alt="test">
                                        </div>
                                        <div class="col-9">
                                            <h3 class="mb-4 ml-4">Nom du projet</h3>
                                            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid amet atque corporis debitis est eum ex fuga impedit quibusdam, rem ullam ut veniam veritatis. Incidunt magnam perferendis quasi quidem sunt.</p>
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
            msg: String
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
                -webkit-filter: brightness(60%); /* Safari 6.0 - 9.0 */
                filter: brightness(60%);
                transform: scale(1.3);
            }
        }
        .modal {
            .modal-dialog{
                margin: 0;
                margin-left: 10%;
                max-width: 80%;
                .modal-content {
                    margin-top: 250px;
                    background-color: #363636;
                    line-height: 26px;
                    .modal-body {
                        color: #FFF;
                        font-weight: 300;
                        img {
                            margin-left: 30px;
                            height: 150px;
                            width: 150px;
                        }
                    }
                }
            }

        }
    }
</style>
