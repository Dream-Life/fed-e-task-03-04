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
                        <!----></button> <button type="button" class="el-button el-button--primary is-plain is-round" style="float: right;">
                        <!----><i class="el-icon-edit"></i><span>写博文</span></button>
                </div>
            </div>
            <div>
                <div class="el-card is-hover-shadow" v-for="(item,index) in $static.bolgs.edges" :key="'bolgs'+index" style="margin-bottom: 20px;">
                    <div class="el-card__header">
                        <div>
                            <div class="el-row">
                                <div class="el-col el-col-16"><span><a style="text-decoration: none; cursor: pointer;"><i class="el-icon-edit-outline"></i>&nbsp;&nbsp; {{item.node.time.split('T')[0]}} 更新
                                        </a></span></div>
                                <div class="el-col el-col-8">
                                    <div style="text-align: right;"><button type="button" class="el-button el-button--text" style="padding: 3px 0px;">
                                            <!----><i class="el-icon-share"></i>
                                            <!----></button>
                                        <!---->
                                        <!---->
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="el-card__body">
                        <div style="font-size: 0.9rem; line-height: 1.5; color: rgb(96, 108, 113);">
                            最近更新 {{item.node.time}}
                        </div>
                        <div style="font-size: 1.1rem; line-height: 1.5; color: rgb(48, 49, 51); padding: 10px 0px 0px;">
                            {{item.node.info}}
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
                            <!---->
                            <li class="number">4</li>
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
	bolgs:allStrapiBolg{
    edges{
      node{
       time
        id
        info
      }
    }
  }
}
</static-query>
<script>
export default {

}
</script>

<style>

</style>
