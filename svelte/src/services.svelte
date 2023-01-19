
<script>
import {Router ,Route ,Link} from "svelte-navigator";
export let servicesRoute;
</script>
<Route>

    <section id="services" class="services section-bg">
        <div class="container">
    
          <div class="section-title">
            <h1 style="text-align: center; padding-top:50px"><strong>Services</strong></h1>
            <p style=" padding-top:50px"><h2><strong>Pick your CV template and get started</strong></h2><p>Our CV templates are designed with your success in mind. They’re all free (with premium features), ATS-friendly, and easy-to-read!</p>
          </div>
    
          <div class="row"style=" padding-top:50px">
            <div class="col-lg-4 col-md-6">
              <div class="icon-box">
                <div class="icon"><i class="bi bi-cash-stack" style="color: #ff689b;"></i></div>
                <h4 class="title"><a href="">Simple</a></h4>
                <p class="description">A simple Curriculum Vitae (CV) layout that was developed for Seniors that have extensive experience in conservative industries such as banking or law.</p>
              </div>
            </div>
            <div class="col-lg-4 col-md-6">
              <div class="icon-box">
                <div class="icon"><i class="bi bi-calendar4-week" style="color: #e9bf06;"></i></div>
                <h4 class="title"><a href="">College</a></h4>
                <p class="description">A college Curriculum Vitae (CV) template for the students that are applying for internships or jobs in academia or research where more than 1 page is needed.</p>
              </div>
            </div>
    
            <div class="col-lg-4 col-md-6" data-wow-delay="0.1s">
              <div class="icon-box">
                <div class="icon"><i class="bi bi-chat-text" style="color: #3fcdc7;"></i></div>
                <h4 class="title"><a href="">Professional</a></h4>
                <p class="description">A professional Curriculum Vitae (CV) template that was developed in collaboration with multiple recruiters to increase your chances of getting your dream job.</p>
              </div>
            </div>
            
    
           
            
          </div>
    
        </div>

      </section>

</Route>

<style>
    
/*--------------------------------------------------------------
# Services
--------------------------------------------------------------*/

.services .icon-box {
  padding: 30px;
  position: relative;
  overflow: hidden;
  border-radius: 10px;
  margin: 0 10px 40px 10px;
  background: #fff;
  box-shadow: 0 10px 29px 0 rgba(68, 88, 144, 0.1);
  transition: all 0.3s ease-in-out;
}

.services .icon-box:hover {
  transform: translateY(-5px);
}

.services .icon {
  position: absolute;
  left: -20px;
  top: calc(50% - 30px);
}

.services .icon i {
  font-size: 64px;
  line-height: 1;
  transition: 0.5s;
}

.services .title {
  
  margin-left: 40px;
  font-weight: 700;
  margin-bottom: 15px;
  font-size: 18px;
 
}

.services .title a {
  color: #111;
}

.services .icon-box:hover .title a {
  color: #e7b549;
}

.services .description {
  font-size: 14px;
  margin-left: 40px;
  line-height: 24px;
  margin-bottom: 0;
}

</style>