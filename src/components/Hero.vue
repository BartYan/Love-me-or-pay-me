<template>
  <div class="wrapper">
        <div class="gifBox">
            <img src="../assets/logo.svg" class="logo" alt="love me or pay me NFT collection" />
            <p>{{ header }}</p>
            <img src="../assets/kittiesGif.gif" class="gif" alt="love me or pay me NFT collection" />
            <p>COMING SOON</p>
            <div class="socialBox">
                <a href="https://www.instagram.com/loveme.or.payme/ " target="_blank">
                    <img src="../assets/insta_biale.svg" class="social" alt="instagram" />
                </a>
                <a href="https://mobile.twitter.com/lovemeorpayNFT" target="_blank">
                    <img src="../assets/TT_biale.svg" class="social" alt="twiter" />
                </a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Hero-Page',
  props: {
    header: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.wrapper {
    width: 100vw;
    height: 100vh;
    padding: 0;
    margin: 0;

    display: flex;
    justify-content: center;
    align-items: center;

    transition: all 0.2s ease-in-out;
    animation: 4s ease-out 0s 1 slideInFromLeft;
    @media (max-width: 1024px) {
        width: 80%;
        margin: 0 auto;
    }
}

.gifBox {
    width: fit-content;
    height: fit-content;

    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.logo {
    width: 100%;
    height: auto;
    animation: beat 3s infinite alternate;
}
p {
    color: #85d638;
    font-size: 18px;
    font-weight: 600;
    margin: 25px 0;
}
.gif {
    display: block;
    width: 50%;
    max-width: 300px;
    height: auto;
    border-radius: 22px;
}
.socialBox {
    display: flex;
    flex-direction: row;
}
.social {
    margin: 0 8px;
    transition: all 0.2s ease-in-out;
}
.social:hover {
    transform: scale(1.1);
}

@keyframes slideInFromLeft {
    0% {
        transform: translateX(-100%);
        -webkit-transform: translateX(-100%);
	/* Safari 4+ */
  -moz-transform: translateX(-100%);
	/* Fx 5+ */
	-o-transform: translateX(-100%);
	/* Opera 12+ */
	-ms-transform: translateX(-100%);
	/*IE11 & Microsoft Edge*/
	transform: translateX(-100%);
    }
    20% {
        transform: translateX(0);
        -webkit-transform: translateX(0);
	/* Safari 4+ */
	-moz-transform: translateX(0);
	/* Fx 5+ */
	-o-transform: translateX(0);
	/* Opera 12+ */
	-ms-transform: translateX(0);
	/*IE11 & Microsoft Edge*/
	transform: translateX(0);
  }
    35% {
        transform: scale(1.1);
        -webkit-transform: scale(1.1);
	/* Safari 4+ */
	-moz-transform:scale(1.1);
	/* Fx 5+ */
	-o-transform:scale(1.1);
	/* Opera 12+ */
	-ms-transform:scale(1.1);
	/*IE11 & Microsoft Edge*/
	transform:scale(1.1);
    }
    50% {
        transform: scale(1);
        -webkit-transform: scale(1);
	/* Safari 4+ */
	-moz-transform:scale(1);
	/* Fx 5+ */
	-o-transform:scale(1);
	/* Opera 12+ */
	-ms-transform:scale(1);
	/*IE11 & Microsoft Edge*/
	transform:scale(1);
    }
    65% {
        transform: scale(1.1);
        -webkit-transform: scale(1.1);
	/* Safari 4+ */
	-moz-transform:scale(1.1);
	/* Fx 5+ */
	-o-transform:scale(1.1);
	/* Opera 12+ */
	-ms-transform:scale(1.1);
	/*IE11 & Microsoft Edge*/
	transform:scale(1.1);
    }
    80% {
        transform: scale(1);
        -webkit-transform: scale(1);
  /* Safari 4+ */
  -moz-transform:scale(1);
  /* Fx 5+ */
  -o-transform:scale(1);
  /* Opera 12+ */
  -ms-transform:scale(1);
  /*IE11 & Microsoft Edge*/
  transform:scale(1);
    }
  }

  @keyframes beat {
	0% { 
		-webkit-transform: scale(1);
  -moz-transform: scale(1);
  -o-transform: scale(1);
  -ms-transform: scale(1);
  transform: scale(1);
}
	15% { transform: scale(1.05); }
	30% { transform: scale(1); }
	100% { transform: scale(1); }
  }
</style>
