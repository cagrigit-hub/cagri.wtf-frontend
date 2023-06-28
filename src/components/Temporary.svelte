
<script lang="ts">
    import monster from "$lib/assets/monstger.png";
</script>

<main class="flex-container col h-screen">
    <div class="flex-container push-bot">
        <img class="image-normal  image-transparent" src={monster} alt="cute-monster" />

        <a href="/">
            <h1 class="title self-centered hover-silver shojumaru  ">
                cagri.wtf
            </h1>
        </a>
       
    </div>
    <p class="greeting-text hover-green-crazy ">
        Hey, my name is Cagri. But people call me ew cagri.wtf?
    </p>
</main>



<style>  
    .shojumaru {
        font-family: 'Shojumaru', cursive;
        
    }
    a {
        text-decoration: none;
    }
    .push-bot {
        margin-bottom: 1rem;
    }
    .greeting-text {
        font-size: 1.5rem;
        font-weight: 500;
        margin: 0;
        padding: 0;
    }
    .col {
      
        flex-direction: column;
    }
    .h-screen {
        height: 75vh;
    }
    
    .image-transparent {
        filter: invert(100%) sepia(0%) saturate(0%) hue-rotate(0deg) brightness(100%) contrast(100%);
    }
    .image-normal {
        width: 4rem;
        height: 4rem;
        margin-right: 1rem;
    }
    .flex-container {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .title {
        font-size: 5rem;
        font-weight: 700;
        margin: 0;
        padding: 0;
    }
    
    .self-centered {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .hover-silver {
        color: #c4c4c4;
    }
    .hover-silver:hover {
        color: #f1f1f1;
    }

    .hover-green-crazy {
        color: #50db50;
        animation: flash 0.5s infinite;
    }
    .hover-green-crazy:hover {
        color: #65ba65;
        animation: flash 0.5s infinite;
    }
    @keyframes flash {
        0% {
            opacity: 1;
        }
        50% {
            opacity: 0.5;
        }
        100% {
            opacity: 1;
        }
    }
    /* responsive mobile */
    @media screen and (max-width: 600px) {
        .title {
            font-size: 3rem;
        }
        .greeting-text {
            font-size: 1rem;
        }
        .image-normal {
            width: 2rem;
            height: 2rem;
        }
    }
    @media screen and (max-width: 400px) {
        .title {
            font-size: 2rem;
        }
        .greeting-text {
            font-size: 0.8rem;
        }
        .image-normal {
            width: 1.5rem;
            height: 1.5rem;
        }
    }
</style>