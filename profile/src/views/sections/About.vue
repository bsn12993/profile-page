<template>
  <div>
    <!-- ======= About Section ======= -->
    <section id="about" class="about">
      <!-- ======= About Me ======= -->
      <div class="about-me container">
        <div class="section-title">
          <h2>{{ $t("menu.about") }}</h2>
          <p class="mt-3">{{ $t("sections.about.title") }}</p>
        </div>

        <div class="row">
          <div class="col-lg-4" data-aos="fade-right">
            <img src="assets/img/avatar.png" class="img-fluid" alt="" />
          </div>
          <div class="col-lg-8 pt-4 pt-lg-0 content" data-aos="fade-left">
            <h3>{{ data.about.profile }}</h3>
            <p class="font-italic" v-show="false">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
            <div class="row">
              <div class="col-lg-6">
                <ul>
                  <li>
                    <i class="icofont-rounded-right"></i>
                    <strong>{{ $t("sections.about.phone") }}: </strong>
                    {{ data.about.phone }}
                  </li>
                  <li>
                    <i class="icofont-rounded-right"></i>
                    <strong>{{ $t("sections.about.city") }}: </strong
                    >{{ data.about.location }}
                  </li>
                </ul>
              </div>
              <div class="col-lg-6">
                <ul>
                  <li>
                    <i class="icofont-rounded-right"></i>
                    <strong>{{ $t("sections.about.email") }}: </strong>
                    {{ data.about.email }}
                  </li>
                  <li>
                    <i class="icofont-rounded-right"></i>
                    <strong>Freelance: </strong> Available
                  </li>
                </ul>
              </div>
            </div>
            <p v-show="false">
              Officiis eligendi itaque labore et dolorum mollitia officiis optio
              vero. Quisquam sunt adipisci omnis et ut. Nulla accusantium dolor
              incidunt officia tempore. Et eius omnis. Cupiditate ut dicta
              maxime officiis quidem quia. Sed et consectetur qui quia
              repellendus itaque neque. Aliquid amet quidem ut quaerat
              cupiditate. Ab et eum qui repellendus omnis culpa magni laudantium
              dolores.
            </p>
          </div>
        </div>
      </div>
      <!-- End About Me -->

      <!-- ======= Counts ======= -->
      <div class="counts container" v-show="false">
        <div class="row">
          <div class="col-lg-3 col-md-6">
            <div class="count-box">
              <i class="icofont-simple-smile"></i>
              <span data-toggle="counter-up">232</span>
              <p>Happy Clients</p>
            </div>
          </div>

          <div class="col-lg-3 col-md-6 mt-5 mt-md-0">
            <div class="count-box">
              <i class="icofont-document-folder"></i>
              <span data-toggle="counter-up">521</span>
              <p>Projects</p>
            </div>
          </div>

          <div class="col-lg-3 col-md-6 mt-5 mt-lg-0">
            <div class="count-box">
              <i class="icofont-live-support"></i>
              <span data-toggle="counter-up">1,463</span>
              <p>Hours Of Support</p>
            </div>
          </div>

          <div class="col-lg-3 col-md-6 mt-5 mt-lg-0">
            <div class="count-box">
              <i class="icofont-users-alt-5"></i>
              <span data-toggle="counter-up">15</span>
              <p>Hard Workers</p>
            </div>
          </div>
        </div>
      </div>
      <!-- End Counts -->

      <!-- ======= Skills  ======= -->
      <div class="skills container">
        <div class="section-title">
          <h2>{{ $t("sections.about.skills") }}</h2>
        </div>
        <div class="row skills-content">
          <div
            class="col-lg-1 mt-4"
            v-for="item in data.skills"
            :key="item.index"
          >
            <SkillItem :item="item" />
          </div>
        </div>
      </div>
      <!-- End Skills -->

      <!-- ======= Testimonials ======= -->
      <div class="testimonials container" v-show="false">
        <div class="section-title">
          <h2>Testimonials</h2>
        </div>

        <div class="owl-carousel testimonials-carousel">
          <div class="testimonial-item">
            <p>
              <i class="bx bxs-quote-alt-left quote-icon-left"></i>
              Proin iaculis purus consequat sem cure digni ssim donec porttitora
              entum suscipit rhoncus. Accusantium quam, ultricies eget id,
              aliquam eget nibh et. Maecen aliquam, risus at semper.
              <i class="bx bxs-quote-alt-right quote-icon-right"></i>
            </p>
            <img
              src="assets/img/testimonials/testimonials-1.jpg"
              class="testimonial-img"
              alt=""
            />
            <h3>Saul Goodman</h3>
            <h4>Ceo &amp; Founder</h4>
          </div>

          <div class="testimonial-item">
            <p>
              <i class="bx bxs-quote-alt-left quote-icon-left"></i>
              Export tempor illum tamen malis malis eram quae irure esse labore
              quem cillum quid cillum eram malis quorum velit fore eram velit
              sunt aliqua noster fugiat irure amet legam anim culpa.
              <i class="bx bxs-quote-alt-right quote-icon-right"></i>
            </p>
            <img
              src="assets/img/testimonials/testimonials-2.jpg"
              class="testimonial-img"
              alt=""
            />
            <h3>Sara Wilsson</h3>
            <h4>Designer</h4>
          </div>

          <div class="testimonial-item">
            <p>
              <i class="bx bxs-quote-alt-left quote-icon-left"></i>
              Enim nisi quem export duis labore cillum quae magna enim sint
              quorum nulla quem veniam duis minim tempor labore quem eram duis
              noster aute amet eram fore quis sint minim.
              <i class="bx bxs-quote-alt-right quote-icon-right"></i>
            </p>
            <img
              src="assets/img/testimonials/testimonials-3.jpg"
              class="testimonial-img"
              alt=""
            />
            <h3>Jena Karlis</h3>
            <h4>Store Owner</h4>
          </div>

          <div class="testimonial-item">
            <p>
              <i class="bx bxs-quote-alt-left quote-icon-left"></i>
              Fugiat enim eram quae cillum dolore dolor amet nulla culpa multos
              export minim fugiat minim velit minim dolor enim duis veniam ipsum
              anim magna sunt elit fore quem dolore labore illum veniam.
              <i class="bx bxs-quote-alt-right quote-icon-right"></i>
            </p>
            <img
              src="assets/img/testimonials/testimonials-4.jpg"
              class="testimonial-img"
              alt=""
            />
            <h3>Matt Brandon</h3>
            <h4>Freelancer</h4>
          </div>

          <div class="testimonial-item">
            <p>
              <i class="bx bxs-quote-alt-left quote-icon-left"></i>
              Quis quorum aliqua sint quem legam fore sunt eram irure aliqua
              veniam tempor noster veniam enim culpa labore duis sunt culpa
              nulla illum cillum fugiat legam esse veniam culpa fore nisi cillum
              quid.
              <i class="bx bxs-quote-alt-right quote-icon-right"></i>
            </p>
            <img
              src="assets/img/testimonials/testimonials-5.jpg"
              class="testimonial-img"
              alt=""
            />
            <h3>John Larson</h3>
            <h4>Entrepreneur</h4>
          </div>
        </div>
      </div>
      <!-- End Testimonials  -->
    </section>
    <!-- End About Section -->
  </div>
</template>
<script>
//Components
import SkillItem from "@/views/components/SkillItem";

export default {
  name: "About",
  props: { data: Object },
  components: { SkillItem },
  data() {
    return {
      skills_left_side: [],
      skills_rigth_side: [],
    };
  },
  created() {},
  methods: {},
};
</script>
