<template>
    <div>
        <h1> Titre 1 </h1>
        <h2> Titre 2 </h2>
        <p> Message : {{message}}</p>
        <p>Seulement premier mot : {{onlyFirstWord}}</p>
        <p>Texte : {{fullText}}</p>
    </div>
</template>
<script>
export default {
    data(){
        return{
            message:"Hello World",
            word:"word",
            hello : "Hello"
        }
    },
    computed:{
        onlyFirstWord(){
            return this.message.split(' ')[0].toUpperCase();
        },
        fullText:{
            //Getter
            get:function(){
            return this.hello + ' ' + this.word;
            },
            //setter
            set:function(newValue){
                const newHelloWorld= newValue.split(' ')
                this.hello=newHelloWorld[0]
                this.word=newHelloWorld[newHelloWorld.length-1]
            }
        }
    }
}
</script>
<style>

</style>