<template>
<Layout>
    <section>
        <div style="min-height: 600px;" class="">
            <div class="el-card is-never-shadow" style="margin-bottom: 20px;">
                <!---->
                <div class="el-card__body">
                    <div class="el-input" style="width: 300px;">
                        <!----><input type="text" autocomplete="off" placeholder="请输入关键字" class="el-input__inner">
                        <!---->
                        <!---->
                        <!---->
                    </div> <button type="button" class="el-button el-button--default is-plain is-circle" style="margin-left: 10px;">
                        <!----><i class="el-icon-search"></i>
                        <!----></button> <button type="button" class="el-button el-button--warning is-plain is-circle" style="margin-left: 10px;">
                        <!----><i class="el-icon-share"></i>
                        <!----></button>
                </div>
            </div>
            <div>
                <div class="el-card is-hover-shadow" style="margin-bottom: 20px;" v-for="(item,index) in $static.codes.edges" :key="'codes'+index">
                    <div class="el-card__header">
                        <div>
                            <div class="el-row">
                                <div class="el-col el-col-16"><span><a style="text-decoration: none; cursor: pointer;"><i class="el-icon-service"></i>&nbsp;&nbsp; canvas-utils
                                        </a></span></div>
                                <div class="el-col el-col-8">
                                    <div style="text-align: right;"><button type="button" class="el-button el-button--text" style="padding: 3px 0px;">
                                            <!----><i class="el-icon-back"></i><span>前往GitHub</span></button> <button type="button" class="el-button el-button--text" style="padding: 3px 0px;">
                                            <!----><i class="el-icon-share"></i>
                                            <!----></button></div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="el-card__body">
                        <div style="font-size: 0.9rem; line-height: 1.5; color: rgb(96, 108, 113);">
                            最近更新 {{item.node.time}}
                        </div>
                        <div style="font-size: 1.1rem; line-height: 1.5; color: rgb(48, 49, 51); padding: 10px 0px 0px;">
                            {{item.node.name}}
                        </div>
                        <div style="font-size: 1.1rem; color: rgb(48, 49, 51); padding: 10px 0px 0px;">
                            <div class="el-row">
                                <div class="el-col el-col-16" style="padding-top: 5px;"><i class="el-icon-star-off el-tooltip" aria-describedby="el-tooltip-7427" tabindex="0" style="margin: 0px 5px 0px 0px;"></i>
                                    {{item.node.fan}}
                                    <i class="el-icon-view el-tooltip" aria-describedby="el-tooltip-5886" tabindex="0" style="margin: 0px 5px 0px 15px;"></i>
                                    {{item.node.look}}
                                    <i class="el-icon-bell el-tooltip" aria-describedby="el-tooltip-7712" tabindex="0" style="margin: 0px 5px 0px 15px;"></i>
                                    {{item.node.tip}}
                                </div>
                                <div class="el-col el-col-8" style="text-align: right;"><span class="el-tag el-tag--danger el-tag--small">{{item.node.tags[0].name}}
                                        <!----></span> <span class="el-tag el-tag--success el-tag--small">{{item.node.tags[1].name}}
                                        <!----></span></div>
                            </div>
                        </div>
                    </div>
                </div>
               
                <div style="text-align: center;">
                    <div class="el-pagination is-background"><button type="button" disabled="disabled" class="btn-prev"><i class="el-icon el-icon-arrow-left"></i></button>
                        <ul class="el-pager">
                            <li class="number active">1</li>
                            <!---->
                            <li class="number">2</li>
                            <li class="number">3</li>
                            <li class="number">4</li>
                            <li class="number">5</li>
                            <!---->
                            <li class="number">6</li>
                        </ul><button type="button" class="btn-next"><i class="el-icon el-icon-arrow-right"></i></button>
                    </div>
                </div>
            </div>
            <!---->
            <div class="el-loading-mask" style="display: none;">
                <div class="el-loading-spinner"><svg viewBox="25 25 50 50" class="circular">
                        <circle cx="50" cy="50" r="20" fill="none" class="path"></circle>
                    </svg>
                    <!---->
                </div>
            </div>
        </div>
    </section>
</Layout>
</template>

<static-query>
query{
	codes:allStrapiCode{
    edges{
      node{
        fan
        id
        look
        name
        tip
        time
        tags{
          name
        }
      }
    }
  }
}
</static-query>

<script>
export default {
    metaInfo: {
        title: 'Code'
    }
}
</script>
