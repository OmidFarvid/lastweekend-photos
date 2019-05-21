<template>
    <section>
        <page-bar></page-bar>
        <div class="kt-portlet">
            <div class="kt-portlet__body">
                <input type="text" class="form-control" placeholder="Search photo - friends - groups...">
                <div class="kt-portlet__head-toolbar">
                </div>
            </div>
            <ul class="nav nav-tabs nav-tabs-line nav-tabs-line-brand nav-tabs-line-2x nav-tabs-line-right nav-tabs-bold text-center"
                role="tablist">
                <li class="nav-item">
                    <a class="nav-link active" data-toggle="tab" href="#all_activity_tab_content"
                       role="tab">
                        All Activity
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" data-toggle="tab" href="#friends_tab_content" role="tab">
                        Friends
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" data-toggle="tab" href="#groups_tab_content" role="tab">
                        Groups
                    </a>
                </li>
            </ul>
            <div class="tab-content">
                <div class="tab-pane active" id="all_activity_tab_content" role="tabpanel">
                    <form class="kt-form kt-form--label-right">
                        <div class="kt-section kt-section--first">
                            <div class="kt-section__body">
                                <div class="form-group kt-form__group row">
                                    <div class="container kt-content">
                                        <div class="row mt-3">
                                            <div class="col-md-5 element-box mt-3" v-for="i in 4" v-bind:key="i">
                                                <div class="kt-portlet">
                                                    <div class="kt-portlet__head">
                                                        <div class="row">
                                                            <div class="col-md-2 text-center">
                                                                <span class="la la-user h2"></span>
                                                            </div>
                                                            <div class="col-md-10">
                                                                <div class="row">
                                                                    <div class="col-md-12 text-left h3 text-black">
                                                                        albert nic
                                                                    </div>
                                                                </div>
                                                                <div class="row">
                                                                    <div class="col-md-12 text-left h3">
                                                                        london
                                                                    </div>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </div>
                                                    <div class="kt-portlet__body">
                                                        <div class="col-12 image-box">
                                                            <img v-bind:src="'resources/images/'+'img'+i+'.jpg'"
                                                                 style="width: 100%;">
                                                            <div class="content">man in laps</div>
                                                        </div>
                                                    </div>
                                                    <div class="kt-portlet__foot">
                                                        <div class="row">
                                                            <div class="col-md-2 h4">
                                                                <span class="la la-comment kt-font-success">35</span>
                                                            </div>
                                                            <div class="col-md-2 h4">
                                                                <span class="la la-heart-o kt-font-danger">443</span>
                                                            </div>
                                                            <div class="col-md-5 offset-3 d-flex h3">
                                                                <a href="#"
                                                                   class="btn btn-outline-success btn-sm btn-icon btn-icon-md">
                                                                    <i class="la la-star-o"></i>
                                                                </a>

                                                                <a href="#"
                                                                   class="btn btn-outline-success btn-sm btn-icon btn-icon-md">
                                                                    <span class="la la-thumbs-o-up"></span>
                                                                </a>
                                                                <a is="router-link" :to="{name: $rns.DOWNLOAD}"
                                                                   class="btn btn-outline-success btn-sm btn-icon btn-icon-md">
                                                                    <i class="la la-download"></i>
                                                                </a>
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </form>
                </div>
                <div class="tab-pane active" id="friends_tab_content" role="tabpanel">
                    <form class="kt-form kt-form--label-right">
                        <div class="kt-section kt-section--first">
                            <div class="kt-section__body">
                                <div class="form-group kt-form__group row">
                                </div>
                            </div>
                        </div>
                    </form>
                </div>
                <div class="tab-pane active" id="groups_tab_content" role="tabpanel">
                    <form class="kt-form kt-form--label-right">
                        <div class="kt-section kt-section--first">
                            <div class="kt-section__body">
                                <div class="form-group kt-form__group row">
                                </div>
                            </div>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import PageBar from "../partials/PageBar";

    export default {
        components: {
            PageBar
        }
    }
</script>

<style scoped>

    .element-box {
        margin-left: 4.444%
    }

    .nav-link.active, .nav-link:hover {
        color: #000000 !important;
        border-color: #000000 !important;
    }

    .nav-tabs.nav-tabs-line.nav-tabs-line-brand.nav-tabs-line-2x {
        border: none !important;
    }

    .kt-portlet {
        border: 1px solid #eeeeee;
    }

    .image-box {
        position: relative;
        margin: 0 auto; /* Center it */
    }

    .image-box .content {
        position: absolute; /* Position the background text */
        bottom: 0; /* At the bottom. Use top:0 to append it to the top */
        background: rgb(0, 0, 0); /* Fallback color */
        background: rgba(0, 0, 0, 0.5); /* Black background with 0.5 opacity */
        color: #f1f1f1; /* Grey text */
        width: 100%; /* Full width */
        padding: 20px; /* Some padding */
    }

    .image-box img {
        vertical-align: middle;
    }
</style>