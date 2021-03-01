{{message | capitalize}}

<div v-bind:id = "rawId | formatId"></div>

filters: {
    capitalize:function(value){
        if(!value) return ''
        value = value.toString()
        return value.chartAt(0).toUpperCase() + value.slice(1)
    }
}


Vue.filters('capitalize',function(value){
    if(!value) return ''
    value = value.toString()
    return value.chartAt(0).toUpperCase() + value.slice(1)
})


new Vue({

})

{{message | filterA | filterB }}