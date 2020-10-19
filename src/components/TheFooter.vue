<template>
  <section id="footer">
    <div class="container">
      <div class="row text-center text-md-left d-flex flex-row justify-content-between">
        <div class="col-md">
          <h5>Quick links</h5>
          <ul class="list-unstyled quick-links">
            <the-footer-item href="#">Home</the-footer-item>
            <the-footer-item href="#">Artigos</the-footer-item>
            <the-footer-item href="#">Comunidade</the-footer-item>
            <the-footer-item href="#">Contato</the-footer-item>
            <the-footer-item href="#">Sobre</the-footer-item>
          </ul>
        </div>

        <div class="col-md">
          <h5>Grupos</h5>
          <ul class="list-unstyled quick-links">
            <the-footer-item href="#">Python</the-footer-item>
            <the-footer-item href="#">JavaScript</the-footer-item>
            <the-footer-item href="#">PHP</the-footer-item>
            <the-footer-item href="#">C/C++</the-footer-item>
            <the-footer-item href="#">Java</the-footer-item>
            <the-footer-item href="#">Linux</the-footer-item>
            <the-footer-item href="#">Vue | React</the-footer-item>
            <the-footer-item href="#">Unity</the-footer-item>
          </ul>
        </div>

        <div class="col-md-auto">
          <h5>Parceiros</h5>
          <ul class="list-unstyled quick-links">
              <the-footer-item href="#">Speaking in English</the-footer-item>
              <the-footer-item href="#">Progresso Aeroespacial</the-footer-item>
              <the-footer-item href="#">Progresso Tech</the-footer-item>
          </ul>
        </div>
        <hr />
      </div>
      <div class="row">
				<div class="col-xs-12 col-sm-12 col-md-12 mt-2 mt-sm-5">
					<ul class="list-unstyled list-inline social text-center">
            <the-footer-social href="#" color="#833AB4">
              <i class="fa fa-instagram"></i>
            </the-footer-social>
            <the-footer-social href="#" color="#4267B2">
              <i class="fa fa-facebook"></i>
            </the-footer-social>
            <the-footer-social href="#" color="#1DA1F2">
              <i class="fa fa-twitter"></i>
            </the-footer-social>
            <the-footer-social href="#" color="#25d366">
              <i class="fa fa-whatsapp"></i>
            </the-footer-social>
            <the-footer-social href="#" color="#D44638">
              <i class="fa fa-envelope"></i>
            </the-footer-social>
					</ul>
				</div>
				<hr>
			</div>	
      <div class="row">
        <div
          class="col-xs-12 col-sm-12 col-md-12 mt-2 mt-sm-2 text-center text-white"
        >
          <p>
            You can never understand everything but you should push yourself to
            understand the system
          </p>
          <p class="h6">
            © All right Reversed. Coding Community,
            {{ new Date().getFullYear() }}
          </p>
        </div>
        <hr />
      </div>
    </div>
  </section>
</template>

<script>
import TheFooterItem from "@/components/TheFooterItem.vue";
import TheFooterSocial from "@/components/TheFooterSocial.vue";

export default {
  name: "TheFooter",

  components: {
    TheFooterItem,
    TheFooterSocial,
  },
};
</script>

<style lang="scss">
section {
  padding: 60px 0;

  .section-title {
    text-align: center;
    color: #007b5e;
    margin-bottom: 50px;
    text-transform: uppercase;
  }
}

#footer {
  background: #121212 !important;

  h5 {
    padding-bottom: 10px;
    margin-bottom: 20px;
    color: #ffffff;
    position: relative;
  }

  h5::after {
    content: '';
    background-color: var(--info);
    position: absolute;
    bottom: 0;
    left: 0;
    width: 50px;
    height: 3px;
  }

}

a {
  color: #ffffff;

  &:hover {
    color: #eeeeee;
  }
}

@media (max-width: 767px) {
  #footer h5 {
    padding-left: 0;
    border-left: transparent;
    padding-bottom: 0px;
    margin-bottom: 10px;
  }

}
</style>