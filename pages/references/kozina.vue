<template>
  <div>
    <Header />

    <BannerKoper />

    <div class="flex spacing__general spacing__inner first-section">
      <div class="flex-grid">
        <div class="flex-grid__col-50">
          <p>Our network of members and volunteers includes a diverse variety of background experiences, ranging from leading Slovenian
            tech companies (Outfit 7, Celtra, Nexto, Reciprocity, Proxima), marketing agencies (Renderspace, Luna, Futura), universities
            (University of Ljubljana, Cornell University, University of London), research institutions (World Debate Institute, Institute
            Jožef Stefan), art collectives (ZEK Crew) and NGOs (CNVOS, Greenpeace, Pro et contra - Institute for the culture of dialogue,
            different labour unions).</p>
        </div>
        <div class="flex-grid__col-50">
          <img src="~/assets/img/tile-image.png" />
        </div>
      </div>
    </div>

    <div class="flex spacing__general spacing__inner first-section">
      <div class="flex-grid">
         <div class="flex-grid__col-50">
          <img src="~/assets/img/tile-image.png" />
        </div>
        <div class="flex-grid__col-50">
          <p>Our projects have received funding by Google DNI (applied to 4 rounds, received 3), NED and American Embassy in Slovenia, and
            have been awarded within the designer/developer community (Brumen award, several Diggit awards ...). Our projects and
            accomplishments are regularly featured in mainstream and indie media and we are often invited to speak at important public events
            at home and abroad.</p>
        </div>
      </div>
    </div>

    <JumboFour />
    <Footer />

  </div>
</template>

<script>
import BannerAbout from "../../components/BannerAbout";
import Footer from "../../components/Footer";
import JumboFour from "../../components/JumboFour";
import Header from "../../components/Header";
import BannerKoper from "../../components/BannerKoper";

export default {
  components: {
      BannerKoper,
      Header,
      BannerAbout,
      Footer,
      JumboFour
  }
}
</script>

<style scoped lang="scss">
    @import './assets/style/common.scss';

    .flex-grid {
      display: flex;

      &__col-50 {
        width: 50%;
      }
    }

    @media (max-width: 900px) {
      .flex-grid {
        display: block;

        &__col-50 {
          width: 100%;
          margin-bottom: 40px;
        }
      }
    }

    .first-section {
      align-items: center;
      margin-left: 20%;
      margin-right: 20%;

      img {
        width: 200px;
        margin-left: 10%;
      }
    }
</style>