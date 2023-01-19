<script>
  	let src ="https://leverageedublog.s3.ap-south-1.amazonaws.com/blog/wp-content/uploads/2019/07/23161145/Resume-in-Computer-Science-01.png";
    let src1 = "https://img.freepik.com/premium-psd/cv-resume-landing-page-design_22994-309.jpg?w=900";

    import {Router ,Route ,Link} from "svelte-navigator";
    import services from "./services.svelte";
    import login from "./login.svelte";
    import Footer from "./lib/footer.svelte";
</script>
<body>

<Router>


  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="/">Resume Builder</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" href="/">Home</a>         </li>
           
          <li class="nav-item">
            <a class="nav-link" href="#">Resume</a>
          </li>
          
          <li class="nav-item">
            <a class="nav-link" href="services">Services</a>
          </li>  
          <li class="nav-item">
            <a class="nav-link" href="login">Login</a>
          </li>            
        </ul>
      </div>
    </div>
  </nav>
<Route>
    <div class="container">
      <div class="row">
        <div class="col">  <center><br><h2 style="padding: 25px;font-size: 55px;">Build a Job Winning 
          <br>Resume for Free</h2>
              <p style="font-size: 25px;">set yourself apart with a modern resume.
              <br>Experts tips, customizable templates and quick pdf 
              <br>download include.</p>
      </center></div>
        <div class="col">
         
          <img src={src} width="700px" height="450px" style = "border-radius: 25px;display: block;    margin-left: auto; margin-right: auto; "  alt="Loading...">
                  </div>
                  <div class="w-100"></div>
              <br><br>

  <div class="col">
    <center><h2 style="font-size: 40px;">How our resume builder works</h2></center>
        <center><p style="font-size: 20px;">Here's the simple process to create a resume:</p></center>
  </div>
  
  <div class="container">
    <br>
    <div class="row">
      <div class="col">
        
        <img src={src1} width="650px" height="450px" style = "border-radius: 25px;display: block;    margin-right: auto; margin-right: auto; "  alt="Loading...">
      </div>

      <br>
      <div class="col">
        <h3 style="padding-left: 50px;">1. Choose your template.</h3>
        <p style="padding-left: 80px;">Browse 30+ professionally designed resume templates to
       
         find the one that speaks to your style and experience. </p>
   
       <h3 style="padding-left: 50px;">2. Enter your information.</h3>
       <p style="padding-left: 80px;">Follow our screen-by-screen prompts as we offer guidance <br>specific to the job to which you’re applying.</p>
   
        <h3 style="padding-left: 50px;">3. Select your content.</h3>
        <p style="padding-left: 80px;">Choose from our prewritten phrases: thousands of customizable <br>bullet points by job title,
         industry and experience level. </p>
   
        <h3 style="padding-left: 50px;">4. Finalize the details.</h3>
        <p style="padding-left: 80px;">Fine-tune your resume design with additional fonts, <br>colors and sections to showcase your personal style. </p>
      </div>
</Route>






   <Route path="services/*servicesRoute" component ={services}/>
   <Route path="login/*loginPage" component ={login}/>
   <Footer/>
  </Router>

</body>


<style>

  .navbar-brand{
      padding-left: 125px;
      font-size: 40px;
      font-weight: 500;
      
  }

  .nav-item{
      font-size: 20px;
      text-align: end;
      padding-left: 25px;
  }
</style>