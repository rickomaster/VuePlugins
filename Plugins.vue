Vue.use(MyPlugin)

new Vue({

})


Vue.use(MyPlugin, {someOption:true})

var Vue = require('vue')
var VueRouter = require('vue-router')

Vue.use(VueRouter)

MyPlugin.install = function(Vue,options){
    // adding global methods
    Vue.myGlobalMethod = function(){
    }

    // add a global asset

    Vue.directive('my-directive',{
        bind(el,binding,vnode,oldVNode){
        }

    })

    Vue.mixin({
        created:function(){
            //injecting some component options
        }
    })
    Vue.prototype.$myMethod = function (methodOptions){
    
}
}

