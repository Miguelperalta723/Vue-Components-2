<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
                <button @click="currentCompontent = 'appQuote' ">Qhote</button>
                <button @click="currentCompontent = 'appRed' ">Red</button>
                <button @click="currentCompontent = 'appGreen' ">Green</button>
                <keep-alive>
                    <component :is="currentCompontent">
                        <p>default content</p>
                    </component>
                </keep-alive>
                
               <!-- <app-quote >
                   <h1 slot="title">Qhote</h1>
                   <p slot="content">a wonderful Quote!</p>
               </app-quote> -->
            </div>
        </div>
    </div>
</template>

<script>
    import Quote from "./components/Quote.vue"
    import Red from "./components/Red.vue"
    import Green from "./components/Green.vue"
    export default {
        data: function(){
            return {
                currentCompontent: "appQuote"
            }
        },
        components: {
            appQuote: Quote,
            appRed: Red,
            appGreen: Green
        }
    }
</script>

<style >
   
</style>
