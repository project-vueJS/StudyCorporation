<template>

<section class='page5'>
    <div class="book">
    <h2>Écouter des évènements</h2>
    <p>Nous pouvons intercepter un événement en ajoutant la<span>v-on</span> directive à l'élément DOM concerné. Disons que nous voulons gérer un clic sur un élément de bouton
    - nous pouvons ajouter ce qui suit à notre modèle Vue:</p>
    <p>La logique avec beaucoup de gestionnaires d’évènements sera très certainement plus complexe, par conséquent, garder votre JavaScript dans la valeur de l’attribut<span>v-on</span> ne sera tout simplement pas faisable. C’est pourquoi v-on peut aussi accepter le nom d’une méthode que vous voudriez appeler.</p>
    <h2>Modificateurs d’évènements</h2>
    <p>C’est un besoin courant que de faire appel à <span>event.preventDefault()</span> ou <span>event.stopPropagation()</span> à l’intérieur d’une déclaration de gestionnaire d’évènements. Bien que nous puissions réaliser ceci aisément à l’intérieur des méthodes, il serait préférable que les méthodes restent purement dédiées à la logique des données au lieu d’avoir à gérer les détails des évènements du DOM.
    Pour résoudre ce problème, Vue propose des modificateurs d’évènements pour <span>v-on</span>. Rappelez-vous que les modificateurs sont des suffixes de directives indiqués par un point.</p>
    <ul>
    <li>.stop</li>
    <li>.prevent</li>
    <li>.capture</li>
    <li>.self</li>
    <li>.once</li>
    <li>.passive</li>
    </ul>
</div>
</section>



</template>


<script>
export default {
  name: 'Mama_'
}

</script>



<style lang="scss">

#app {
  font-family: 'Calligraffitti', cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100vh;
  display: grid;
  place-items: center;

    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        }


        section{
            
        .book{
            width: 30%;
            height: 80%;
            position: relative;
            padding: 30px;
            box-shadow: 0 4px 8px rgba($color: #000000, $alpha: 0.2);
            
            @import url('https://fonts.googleapis.com/css2?family=Calligraffitti&display=swap');
            span {
                    padding: 10px;
                    background-color: rgba(228, 228, 228, 0.486);
                    color: black;
                }
                    h2{
                        color: #f25417;
                    }

                        li{
                            list-style-type: disc;
                            margin-left: 40%;
                        }

            }
    }
}
</style>
