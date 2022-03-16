<template>

    <section>
        <h2>Syntaxe Vue</h2>

        <div class="pres">
            <h3>Introduction</h3>
            <p>Vue.js utilise une syntaxe de template basée sur le HTML qui vous permet de lier déclarativement le DOM
                rendu aux données de l’instance sous-jacente de Vue. Tous les templates de Vue.js sont du HTML valide
                qui peut être interprété par les navigateurs et les interpréteurs HTML conformes aux spécifications.</p>

        </div>

        <div class="synt">
            <h3>Syntaxe :</h3>
        <h5>Template = Code html :</h5>
            <pre><code class="language-html">
&lt;template>
&lt;div class="hello">
    &lt;h1>Hello World&lt;/h1>
        &lt;p>
            For a guide and recipes on how to configure / customize this project,
            check out the
        &lt;a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation&lt;/a>.
        &lt;/p>
    &lt;ul>
        &lt;li>&lt;a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router&lt;/a>&lt;/li>
        &lt;li>&lt;a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex&lt;/a>&lt;/li>
    &lt;/ul>
&lt;/div>
&lt;/template>


&lt;script>
    import Prism from "prismjs";
    import "prismjs/themes/prism.css"; // you can change
    export default {
        name: 'app',
        data() {
            return {
                //
            };
        },
        // mounted
        mounted() {
            window.Prism = window.Prism || {};
            window.Prism.manual = true;
            Prism.highlightAll(); // highlight your code on mount
        }
    };
&lt;/script>

&lt;style lang="scss">
    section {

        width : 35%;
        border : black solid 1px;
        box-shadow : 2px 2px 8px grey;
        margin : 0 auto;

        font-size: 8px;

        h2, h3, h4, p{
            font-size: 16px;
            text-align : center;
        }

        p {
            color: black;
            margin: 0 20px;
        }
    }
&lt;/style>



</code></pre>



</div>


</section>
</template>


<script>
    import Prism from "prismjs";
    import "prismjs/themes/prism.css"; // you can change
    export default {
        name: 'app',
        data() {
            return {
                //
            };
        },
        // mounted
        mounted() {
            window.Prism = window.Prism || {};
            window.Prism.manual = true;
            Prism.highlightAll(); // highlight your code on mount
        }
    };
</script>

<style lang="scss">
    section {

        width : 35%;
        border : black solid 1px;
        box-shadow : 2px 2px 8px grey;
        margin : 0 auto;

        font-size: 8px;

        h2, h3, h4, p{
            font-size: 16px;
            text-align : center;
        }

        p {
            color: black;
            margin: 0 20px;
        }
    }
</style>