<template>
  <div class="score">
    <h1>This is an score page</h1>
    <p>{{ score }}</p>
  </div>
</template>
<script>
       export default {
        name: 'score',
        props: ['scores'],
        data() {
            return {}
        },
        methods: {
            dataReset() {
                this.$parent.$data.scores = [];
            }
        }
    };
</script>
<script>
        export default {
            data() {
                return {
                    
                };
            },
        computed:{
            score(){
                return this.$store.getters.score
            }
        }
    };
    </script>