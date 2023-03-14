<template>
  <nav id="top" class="nav">
    <div class="nav__image">
      <img src="@/assets/univers-plaid-logo.svg" alt="univers plaid logo">
    </div>
    <div  class="nav__menu" id="burder-menu">
      <ul>
        <li class="page-link">
          <a href="/">Notre collection</a>
        </li>
        <li  class="page-link" id="dropdown">
          <span>
            Nos plaid classiques
            <i class="fa-solid fa-chevron-down"></i>
          </span>
          <div>
            <ul>
              <li>Pull plaid</li>
              <li>Plaid disney</li>
              <li>Plaid animaux</li>
              <li>Plaid kangourou</li>
              <li>Plaid sirène</li>
              <li>Plaid imprimé</li>
            </ul>
            <a href="#">En voir plus</a>
          </div>
        </li>
        <li class="page-link" id="dropdown">
        <span>
          Nos plaid spéciaux
          <i class="fa-solid fa-chevron-down"></i>
        </span>
        <div>
          <ul>
            <li>Couverture chauffante</li>
            <li>Plaid canapé</li>
            <li>Plaid cocooning</li>
            <li>Plaid grosse maille</li>
            <li>Plaid enfant</li>
            <li>Plaid bébé</li>
          </ul>
          <a href="#">En voir plus</a>
        </div>
        </li>
      </ul>
      
      <hr>

      <div>
        <i id="cart" class="fa-solid fa-cart-shopping"></i>
        <i class="fa-solid fa-user"></i>
      </div>
    </div>

    <div id="hamburger" class="nav__hamburger hamburger--elastic js-hamburger">
      <div class="hamburger-box">
        <div class="hamburger-inner"></div>
      </div>
    </div>
  </nav>
  <main class="content">
    <header class="content__banner" data-aos="fade-up">
      <div class="content__banner__text">
        <h1>Offrez-vous le plaid réconfortant dont vous avez besoin !</h1>
        <p>Nous avons une grande variété de <strong>modèles</strong>, de <strong>couleurs</strong>, et de <strong>textures</strong> pour s'adapter à tous les goûts et à tous les styles.</p>
        <span>-10% maintenant avec le code dcg10</span>
      </div>
      <form class="content__banner__cta">
        <input type="text" placeholder="Quel plaid vous ferez plaisir ?">
        <button type="reset">Rechercher</button>
      </form>
    </header>

    <section class="content__section content__famous">
      <h2>Nos coups de coeur</h2>
      <div class="content__famous__cards">
        <FamousCard data-aos="fade-right" position="div1" cover="vedette_2.webp"/>
        <FamousCard data-aos="fade-right" position="div2" cover="vedette_4.webp"/>
        <FamousCard data-aos="fade-up" position="div3" cover="vedette_1.webp"/>
        <FamousCard data-aos="fade-left" position="div4" cover="vedette_3.webp"/>
        <FamousCard data-aos="fade-left" position="div5" cover="vedette_5.webp"/>
      </div>
    </section>

    <section class="content__section content__collections">
      <h2>Nos collections<span>Univers Plaid</span></h2>
      <div class="content__collections__cards">
        <CollectionCard 
          data-aos="fade-right"
          title="Par couleur ou univers" 
          description="Sublimez vos intérieurs avec nos plaids de toutes les couleurs, bleu, vert, jaune.. Ou offrez-vous simplement le plaid de votre univers favori."
          cover="collection_1.webp"
        />
        <CollectionCard
          data-aos="fade-up"
          title="Pour enfant" 
          description="Les plaids ont envahi nos intérieurs. Un plaid pour vos enfants avec des motifs dinosaures ou baby shark."
          cover="collection_2.webp"
        />
        <CollectionCard
          data-aos="fade-left"
          title="Par bébé" 
          description="Spécialement conçu pour les bébés, nos plaids sont incroyablement doux."
          cover="collection_3.webp"
        />
      </div>
    </section>

    <section class="content__section content__about">
        <img src="@/assets/univers-plaid-about.webp" alt="family image" data-aos="fade-right">
        <div data-aos="fade-left">
          <h3>Qui sommes-nous ?</h3>
          <p>Chez <strong>Univers Plaid</strong>, nous sommes convaincus que chacun mérite de se blottir dans un <strong>plaid confortable</strong> après une longue journée de travail ou pour une soirée cocooning à la maison. C'est pourquoi nous mettons tout en œuvre pour offrir à nos clients des <strong>produits de qualité supérieure</strong> à des <strong>prix abordables</strong>, avec un <strong>service client irréprochable</strong>. Nous n’avons qu’un seul objectif : <strong>vous chouchouter</strong>.</p>
          <a href="#">Découvrir nos produits</a>
        </div>
    </section>

    <section class="content__section content__service" data-aos="fade-up">
      <ServiceCard title="Livraison offerte" description="Dès 50€ d'achat" icon="camion.svg"/>
      <ServiceCard title="Satisfait ou remboursé" icon="money-back.svg"/>
      <ServiceCard title="Service client" description="Réactif et à l'écoute" icon="service-client.svg"/>
    </section>

    <section class="content__section content__newsletter" data-aos="fade-up">
      <div>
        <img src="@/assets/envelope.svg" alt="">
        <h3>Newsletter</h3>
        <p>Inscrivez-vous à notre newsletter et profitez de 15% sur votre première commande.</p>
        <form>
          <input type="text" placeholder="Votre@email.com">
          <button type="reset">S'inscrire</button>
        </form>
      </div>
    </section>

    <footer class="content__footer">
      <div class="content__footer__top-part">
        <div>
          <img src="@/assets/univers-plaid-logo.svg" alt="logo univers plaid">
          <ul class="company">
            <li>Univers Plaid</li>
            <li>Bernissart, Belgique</li>
            <li>contact@univers-plaid.com</li>
            <li>07.80.99.65.35</li>
          </ul>
        </div>

        <div>
          <h4>Liens Utiles</h4>
          <ul>
            <li><a href="#">Accueil</a></li>
            <li><a href="#">Notre Collection</a></li>
            <li><a href="#">Mon Compte</a></li>
            <li><a href="#">FAQs</a></li>
            <li><a href="#">Nous contacter</a></li>
            <li><a href="#">Blog</a></li>
          </ul>
        </div>

        <div>
          <h4>à propos</h4>
          <ul>
            <li><a href="#">Mentions légales</a></li>
            <li><a href="#">Conditions générales de vente</a></li>
            <li><a href="#">Politique de confidentialité</a></li>
            <li><a href="#">Politique de remboursement</a></li>
            <li><a href="#">Politique de livraison</a></li>
            <li><a href="#">Rétractation</a></li>
          </ul>
        </div>

        <div class="top-button">
          <a href="#top"><i class="fa-solid fa-arrow-up"></i></a>
        </div>
      </div>

      <hr>

      <div class="content__footer__bottom-part">
        <span>© Copyright Univers-Plaid™ 2023 · Tous droits réservés</span>
        <img src="@/assets/credit-cards.webp" alt="credit card">
      </div>
    </footer>
  </main>
</template>

<script>
  import FamousCard from '@/components/FamousCardComponent.vue';
  import CollectionCard from '@/components/CollectionCardComponent.vue';
  import ServiceCard from '@/components/ServiceComponent.vue';
  import AOS from 'aos';
  import 'aos/dist/aos.css';

  export default {
    name: 'App',
    components: {
      FamousCard,
      CollectionCard,
      ServiceCard
    },
    mounted() {
      AOS.init({
        duration: 1000,
      });
      const burger = document.getElementById('hamburger');
      const menu = document.getElementById('burder-menu');
      const dropdowns = document.querySelectorAll('#dropdown');

      burger.addEventListener('click', () => {
        burger.classList.toggle('is-active');
        menu.classList.toggle('is-active');
      });
      dropdowns.forEach(dropdown => {
        dropdown.addEventListener('click', () => {
          dropdown.classList.toggle('is-active');
        });
      });
    }
  }
</script>

<style lang="scss" scoped>
$pseudo-border: #0A3969;
  .nav {
    height: 10vh; 
    margin: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 1rem;
    box-shadow: 0px 5px 20px rgba(0, 0, 0, 0.15);

    &__image {
      height: 6vh;

      img {
        height: 100%;
      }
    }

    &__menu {
      display: none;

      @keyframes openMenu {
        0% {
          opacity: 0;
          transform: scaleY(0);
          transform-origin: top;
        }
        100% {
          opacity: 1;
          transform: scaleY(1);
          transform-origin: top;
        }
      }

      @media screen and (min-width: 1100px)
      {
        display: flex;
        border: 2px  red;
        width: 100%;
        justify-content: space-between;
        align-items: center;

        ul {
          list-style: none;
          display: flex;
          align-items: flex-start;
          justify-content: center;
          gap: 30px;
          width: 90%;

          @media screen and (min-width: 1024px) {
            font-size: 16px;
          }

          li {
            color: #0A3969;
            font-weight: bold;
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            justify-content: center;
            cursor: pointer;

            &.is-active {
              position: relative;
              div{
                display: flex;
                flex-direction: column;
                align-items: flex-start;
                justify-content: space-between;
                position: absolute;
                background-color: #ffffff;
                top: 100%;
                z-index: 1;
                width: 120%;
                padding: 1rem;
                gap: 20px;

                ul {
                  display: flex;
                  flex-direction: column;
                }
              }
            }

            &.page-link {
              position: relative;

              &::after {
                content: '';
                position: absolute;
                width: 100%;
                transform: scaleX(0);
                height: 2px;
                bottom: -5px;
                left: 0;
                background-color: #0A3969;
                transform-origin: bottom right;
                transition: transform 0.25s ease-out;
              }

              &:hover::after {
                transform: scaleX(1);
                transform-origin: bottom left;
              }
            }

            div {
              display: none;
              flex-direction: column;
              font-size: 16px;
              margin: 30px 0;

              ul {
                gap: 15px;
                margin-bottom: 10px;
              }
            }
            
            a {
              text-decoration: none;
              color: #0A3969;
            }
          }
        }

        hr {
          display: none;
        }
      }

      &.is-active {
        display: flex;
        flex-direction: column-reverse;
        align-items: center;
        justify-content: flex-end;
        padding: 10vh 0;
        width: 100vw;
        min-height: 90vh;
        position: absolute;
        z-index: 1;
        background-color: #ffffff;
        top: 10vh;
        left: 0;
        font-size: 20px;
        animation: openMenu .75s;

        hr {
          width: 80%;
          border: 1px solid #0A3969;
          border-radius: 10px;
          margin: 25px 0;
        }
        
        ul {
          list-style: none;
          display: flex;
          flex-direction: column;
          align-items: flex-start;
          justify-content: center;
          gap: 30px;

          @media screen and (min-width: 1024px) {
            font-size: 28px;
          }

          li {
            color: #0A3969;
            font-weight: bold;
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            justify-content: center;
            cursor: pointer;

            &.page-link {
              position: relative;

              &::after {
                content: '';
                position: absolute;
                width: 100%;
                transform: scaleX(0);
                height: 2px;
                bottom: -5px;
                left: 0;
                background-color: #0A3969;
                transform-origin: bottom right;
                transition: transform 0.25s ease-out;
              }

              &:hover::after {
                transform: scaleX(1);
                transform-origin: bottom left;
              }
            }

            div {
              display: none;
              flex-direction: column;
              font-size: 16px;
              margin: 30px 0;

              ul {
                gap: 15px;
                margin-bottom: 10px;
              }
            }
            
            a {
              text-decoration: none;
              color: #0A3969;
            }
          }
        }

      }
      
      div {
        display: flex;
        gap: 30px;
        color: #0A3969;
        font-size: 24px;

        @media screen and (min-width: 1024px) {
          font-size: 40px;
        }

        @media screen and (min-width: 1100px) {
          font-size: 24px;
        }
        
        i {
          cursor: pointer;
        }

        #cart {
          position: relative;

          &::after {
            content: "0";
            position: absolute;
            bottom: -10px;
            right: -10px;
            display: flex;
            align-items: center;
            justify-content: center;
            width: 15px;
            aspect-ratio: 1/1;
            font-size: 12px;
            font-weight: bold;
            background-color: #FF8282;
            color: white;
            border-radius: 50%;
            padding: 2px;

            @media screen and (min-width: 1024px) {
              font-size: 20px;
              width: 25px;
              bottom: -15px;
            }

            @media screen and (min-width: 1100px) {
              font-size: 12px;
              width: 15px;
              bottom: -10px;
            }
          }
        }
      }

      ul {
        li i {
          transform: rotate(0deg);
        }
        li.is-active {

          &.page-link:hover::after {
            transform: scaleX(0);
            transform-origin: bottom left;
          }

          div {
            display: flex;
          }

          i {
            transform: rotate(180deg);
          }
        }
      }
    }

    &__hamburger {
      font: inherit;
      display: inline-block;
      overflow: visible;
      margin: 0;
      padding: 15px;
      cursor: pointer;
      transition-timing-function: linear;
      transition-duration: .15s;
      transition-property: opacity,filter;
      text-transform: none;
      color: inherit;
      border: 0;
      background-color: transparent;

      @media screen and (min-width: 1100px)
      {
        display: none;
      }

      .hamburger-box {
        position: relative;
        display: inline-block;
        width: 40px;
        height: 24px;

        @media screen and (min-width: 1024px) {
          width: 50px;
          height: 30px;
        }

        .hamburger-inner {
          top: 0;
          left: 0;
          transition-timing-function: cubic-bezier(.68,-.55,.265,1.55);
          transition-duration: .275s;

          &::before, &::after {
            display: block;
            content: "";
          }

          &::before {
            top: 10px;

            @media screen and (min-width: 1024px) {
              top: 13px;
            }
          }

          &::after {
            top: 20px;

            @media screen and (min-width: 1024px) {
              top: 26px;
            }
          }
        }

        .hamburger-inner, .hamburger-inner:after, .hamburger-inner:before {
          position: absolute;
          width: 40px;
          height: 4px;
          transition-timing-function: ease;
          transition-duration: .15s;
          transition-property: transform;
          border-radius: 4px;
          background-color: #0A3969;

          @media screen and (min-width: 1024px) {
            height: 5px;
            width: 100%;
          }
        }
      }

      &.is-active .hamburger-inner {
        transition-delay: 75ms;
        transform: translate3d(0,10px,0) rotate(135deg);

        &::before {
          transition-delay: 0s;
          opacity: 0;
        }

        &::after {
          transition-delay: 75ms;
          transform: translate3d(0,-20px,0) rotate(-270deg);

          @media screen and (min-width: 1024px) {
            transform: translate3d(0,-20px,0) rotate(-270deg) translateX(-4px);
          }
        }
      }
    }
  }

  .content {
    width: 100vw;

    &__banner {
      position: relative;
      width: 100%;
      height: 70vh;
      background-image: url("@/assets/responsive-hero.png");
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      @media screen and (min-width: 768px) {
        background-image: url("@/assets/desktop-hero.png");
      }

      &__text {
        color: #ffffff;
        text-align: center;
        width: 100%;
        font-weight: 100;
        padding: 10px;

        @media screen and (min-width: 768px) {
          width: 70%;
        }

        @media screen and (min-width: 1024px) {
          width: 80%;
        }

        @media screen and (min-width: 1100px) {
          width: 60%;
        }

        h1 {
          font-size: 32px;
          font-weight: bold;
          margin-bottom: 30px;
          
          @media screen and (min-width: 1024px) {
            font-size: 48px;
          }

          @media screen and (min-width: 1100px) {
            font-size: 40px;
          }
        }

        p {
          font-size: 20px;
          margin-bottom: 50px;
          font-family: sans-serif;

          @media screen and (min-width: 1024px) {
            font-size: 28px;
          }

          @media screen and (min-width: 1100px) {
            font-size: 20px; 
          }
        }

        span {
          font-size: 16px;
          font-weight: 100;
          font-family: sans-serif;
          text-transform: uppercase;

          @media screen and (min-width: 1024px) {
            font-size: 20px;
          }

          @media screen and (min-width: 1100px) {
            font-size: 16px;
          }
        }
      }

      &__cta {
        position: absolute;
        bottom: -10%;
        background-color: #BCCEEA;
        padding: 1rem;
        border-radius: 10px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 15px;
        width: 90%;

        @media screen and (min-width: 1024px) {
          flex-direction: row;
          width: 80%;
          bottom: -40px;
        }

        @media screen and (min-width: 1100px) {
          width: 60%;
        }

        input {
          border: none;
          padding: .8rem 1rem;
          background-color: #ffffff;
          width: 100%;
          border-radius: 10px;
          display: flex;
          align-items: center;
          justify-content: space-between;

          @media screen and (min-width: 1024px) {
            font-size: 20px;
            padding: 1rem;
          }
          @media screen and (min-width: 1100px) {
            font-size: 16px;
          }

          &:focus {
            outline: none;
          }

          &::placeholder {
            color: #0A3969;
          }
        }

        button {
          padding: 1em 2rem;
          background-color: #ffffff;
          border-radius: 10px;
          border: none;
          color: #0A3969;
          font-family: sans-serif;
          font-weight: 900;
          cursor: pointer;

          @media screen and (min-width: 1024px) {
            font-size: 20px;
            padding: 1rem 2rem;
          }

          @media screen and (min-width: 1100px) {
            font-size: 16px; 
          }

          &:hover {
            background-color: #0A3969;
            color: #ffffff;
          }
        }
      }
    }

    &__section {
      margin: 100px 0;

      @media screen and (min-width: 600px) {
        width: 80%;
        margin: 100px auto;
      }

      @media screen and (min-width: 1024px) {
        margin: 200px auto;
      }

      @media screen and (min-width: 1100px) {
        width: 90%;
        margin: 200px auto;
      }

      @media screen and (min-width: 1200px) {
        width: 80%;
      }

      h2 {
        width: fit-content;
        margin: 60px auto;
        position: relative;
        text-align: center;
        font-size: 28px;
        font-weight: bold;
        color: #0A3969;
        font-family: 'Yeseva One', cursive;

        @media screen and (min-width: 1024px) {
          font-size: 32px;
          margin: 100px auto;
        }

        @media screen and (min-width: 1100px) {
          font-size: 32px;   
        }

        &::after, &::before {
          content: "";
          position: absolute;
          width: 20px;
          height: 20px;
          @media screen and (min-width: 1024px) {
            width: 30px;
            height: 30px;
          }
        }

        &::after {
          bottom: -5px;
          right: -10px;
          border-bottom: 3px solid $pseudo-border;
          border-right: 3px solid $pseudo-border;

          @media screen and (min-width: 1024px) {
            border-width: 4px;
            bottom: -10px;
            right: -20px;
          }
        }
        
        &::before {
          top: -5px;
          left: -10px;
          border-top: 3px solid $pseudo-border;
          border-left: 3px solid $pseudo-border;

          @media screen and (min-width: 1024px) {
            border-width: 4px;
            top: -10px;
            left: -20px;
          }
        }
      }
    }

    &__famous {
      margin-top: 150px;

      &__cards {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-template-rows: repeat(4, 1fr);
        grid-column-gap: 15px;
        grid-row-gap: 15px;
        place-items: center;
        width: 90%;
        margin: auto;

        .div1 { grid-area: 1 / 1 / 2 / 2; }
        .div2 { grid-area: 1 / 2 / 2 / 3; }
        .div3 { grid-area: 2 / 1 / 4 / 3; }
        .div4 { grid-area: 4 / 1 / 5 / 2; }
        .div5 { grid-area: 4 / 2 / 5 / 3; }

        @media screen and (min-width: 1024px) {
          display: grid;
          grid-template-columns: repeat(4, 1fr);
          grid-template-rows: repeat(2, 1fr);
          grid-column-gap: 20px;
          grid-row-gap: 20px;
          width: 100%;

          .div1 { grid-area: 1 / 1 / 2 / 2; }
          .div2 { grid-area: 2 / 1 / 3 / 2; }
          .div3 { grid-area: 1 / 2 / 3 / 4; }
          .div4 { grid-area: 1 / 4 / 2 / 5; }
          .div5 { grid-area: 2 / 4 / 3 / 5; }
        }
      }
    }

    &__collections {
      width: 100vw;

      @media screen and (min-width: 600px) {
        width: 80%;
        margin: auto;
      }

      h2 {
        display: flex;
        gap: 15px;
      }

      h2 span {
        display: none;

        @media screen and (min-width: 1024px) {
          display: block;
          font-family: 'Yeseva One', cursive;
        }
      }

      &__cards {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 50px;

        @media screen and (min-width: 600px) {
          width: 60%;
          margin: auto;
        }

        @media screen and (min-width: 1024px) {
          flex-direction: row;
          width: 100%;
          gap: 30px;
        }
        @media screen and (min-width: 1200px) {
          gap: 50px;
        }
      }
    }

    &__about {
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;

      @media screen and (min-width: 1024px) {
        justify-content: flex-start;
      }

      img {
        width: 150%;

        @media screen and (min-width: 600px) {
          width: 80%;
        }

        @media screen and (min-width: 1024px) {
          width: 60%; 
        }

        @media screen and (min-width: 1200px) {
          width: 50%;
        }
      }

      div {
        background-color: rgba(188, 206, 234, 0.8);
        position: absolute;
        bottom: -25vh;
        width: 100vw;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: center;
        padding: 3rem;

        @media screen and (min-width: 600px) {
          width: 80%;
          bottom: -25vh;
        }

        @media screen and (min-width: 1024px) {
          width: 70%;
          height: 80%;
          top: 10%;
          right: 0;
          padding: 2rem 4rem;
        }

        h3 {
          font-size: 28px;
          font-weight: bold;
          color: #0A3969;
          font-family: 'Yeseva One', cursive;
          margin: 25px 0;
          @media screen and (min-width: 1024px) {
            font-size: 24px;
          }
        }

        p {
          color: #0A3969;
          margin: 25px 0;
          @media screen and (min-width: 1024px) {
            font-size: 16px;
          }
        }

        a {
          padding: 1rem 2rem;
          width: 100%;
          display: flex;
          align-items: center;
          justify-content: center;
          color: #FFFFFF;
          margin: 25px 0;
          text-decoration: none;
          background: #829ADE;
          border-radius: 10px;

          @media screen and (min-width: 1024px) {
            font-size: 16px;
            width: auto;
          }

          &:hover {
            background: #0A3969;
          }
        }
      }
    }

    &__service {
      background-color: #C9D8EE;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      gap: 50px;
      padding: 50px 0;
      margin-top: 40vh;
      margin-bottom: 0;

      @media screen and (min-width: 768px) {
          margin-top: 30vh;
      }

      @media screen and (min-width: 1024px) {
        flex-direction: row;
        align-items: flex-start;
        margin-top: 15vh;
        padding: 0;
        gap: 0;
        width: 100vw;
      }

      @media screen and (min-width: 1200px) {
        padding: 0 4rem;
      }
    }

    &__newsletter {
      background-image: url("@/assets/mobile-newsletter.png");
      background-size: cover;
      background-repeat: no-repeat;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: #FFFFFF;
      width: 100vw;
      padding: 100px 25px;
      margin: 0;

      @media screen and (min-width: 768px) {
        background-image: url("@/assets/desktop-newsletter.png");
      }

      div {
        width: 100%;

        @media screen and (min-width: 768px) {
          width: 70%;
        }

        @media screen and (min-width: 1200px) {
          width: 40%;
        }

        img {
          width: 50px;

          @media screen and (min-width: 1024px) {
            width: 60px;
          }
        }

        h3 {
          font-size: 24px;
          font-family: 'Yeseva One', cursive;
          margin: 15px 0;

          @media screen and (min-width: 1024px) {
            font-size: 28px;
            margin: 30px 0;
          }
        }

        p {
          @media screen and (min-width: 1024px) {
            font-size: 20px;
          }
        }
        
        form {
          margin-top: 40px;
          display: flex;
          flex-direction: column;
          align-items: center;
          justify-content: center;
          gap: 20px;
          @media screen and (min-width: 1024px) {
            margin-top: 50px;
            gap: 30px;
          }

          input {
            border: none;
            padding: .8rem 1rem;
            background-color: rgba(7, 30, 54, 0.5);
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: space-between;
            color: #ffffff;
            border: 2px solid #FFFFFF;
            @media screen and (min-width: 1024px) {
              font-size: 20px;
              padding: .8rem 2rem;
            }

            &:focus {
              outline: none;
            }

            &::placeholder {
              color: #FFFFFF;
            }
          }

          button {
            padding: 1em 3rem;
            background-color: #ffffff;
            border-radius: 10px;
            border: none;
            color: #0A3969;
            font-family: sans-serif;
            font-weight: 900;
            cursor: pointer;

            @media screen and (min-width: 1024px) {
              font-size: 16px;
              padding:  .8rem 4rem;
            }

            &:hover {
              background-color: #0A3969;
              color: #ffffff;
            }
          }
        }
      }
    }

    &__footer {
      background-color: #C9D8EE;
      padding: 50px 40px;

      @media screen and (min-width: 1024px) {
          padding: 3rem;
      }

      &__top-part {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: center;
        gap: 50px;

        @media screen and (min-width: 1024px) {
          flex-direction: row;
          align-items: flex-start;
          justify-content: space-between;
          width: 100%;

          div {
            width: 25%;
          }
        }

        img {
          width: 200px;
        }

        h4 {
          font-size: 24px;
          font-family: 'Yeseva One', cursive;
          color: #0A3969;
          text-transform: uppercase;

          @media screen and (min-width: 1024px) {
            margin-top: 20px;
          }
        }

        .company {
          margin-top: 50px;

          @media screen and (min-width: 1024px) {
            margin-top: 70px;
          }
        }

        ul {
          margin-top: 15px;
          list-style: none;
          color: #0A3969;

          li {
            line-height: 1.75rem;

            a {
              color: #0A3969;
              text-decoration: none;
            }
          }
        }

        .top-button {
          background-color: #0A3969;
          height: 60px;
          width: 60px;
          display: flex;
          align-items: center;
          justify-content: center;
          border-radius: 50%;
          margin: 0 auto 25px;
          margin-top: 20px;

          a {
            color: #C9D8EE;
            font-size: 32px;
          }
        }
      }

      hr {
        border: 1px solid #0A3969;
        border-radius: 10px;
        margin: 25px 0;
      }

      &__bottom-part {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: center;
        gap: 20px;

        @media  screen and (min-width: 1024px) {
          flex-direction: row;
          justify-content: space-between;
          align-items: center;
        }

        span {
          color: #0A3969;
          width: 90%;
        }

        img {
          width: 250px;
        }
      }
    }
  }
</style>
