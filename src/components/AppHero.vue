<script>

export default {
    name: 'AppHero',
}

</script>

<template>

    <div id="jumbotron">  
        <div class="jumbo-text">
            <h2>
                Vue utilizzato dentro Vite
            </h2>
    
            <p>
                Testo del jumbotron
            </p>
    
            <button>
                Scopri di più
            </button>
        </div>
    </div>

</template>

<style>

#jumbotron {
    display: flex;
    flex-flow: column;
    justify-content: flex-end;

    position: relative;

    height: 600px;
    
    padding: 20px;

    background-image: url('https://immagini.alvolante.it/sites/default/files/styles/anteprima_lunghezza_640/public/news_galleria/2024/02/ferrari-sf24-formula-1_1.jpg');
    background-size: cover;
    background-position: bottom;

    margin-bottom: 2em;
}

#jumbotron::before {
    content: '';

    position: absolute;
    top: 0;
    left: 0;
    z-index: 0;

    width: 100%;
    height: 100%;

    background-image: linear-gradient(#00000000, #000000ff);
}

#jumbotron .jumbo-text {
    z-index: 1;

    padding: 20px 0;
}

</style>