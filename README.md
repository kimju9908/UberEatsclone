# UberEatsclone
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>UberEats 스타일 헤더 및 사이드바</title>
    <style>
      * {
        margin: 0;
        padding: 0;
      }

      body {
        font-family: Arial, sans-serif;
      }

      main {
        height: 100vh;
        display: flex;
        justify-content: flex-start; 
        align-items: flex-start; 
        background-image: url("./images/mainbackground.webp");
        background-size: cover;
        background-position: center;
        padding: 0 20px; 
      }

      .sentence {
    padding-bottom: 0;
    color: black;
    line-height: 36px;
    font-size: 28px;
    font-weight: 700;
    text-align: left;
    text-decoration: none; 
    }

      .sentence1 {
        color: black;
        font-size: 16px;
        text-decoration: underline;
        line-height: 20px;
        font-weight: 500;
        cursor: pointer;
        margin-top: 8px;
        text-align: left; 
      }

     
      .main-content h1 {
        margin-top: 350px;
        line-height: 64px;
        font-size: 52px;
        font-weight: bold;
        color: black;
        margin-bottom: 40px;
      }

      
      .main-content {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        text-align: left;
        padding: 20px;
        border-radius: 8px;
        max-width: 839px;
        width: 100%;
      }

      .action-group {
        align-items: center;
        display: flex;
        gap: 10px;
        width: 100%;  
        justify-content: flex-start;
      }
      .input {
        background-image: url("./images/text.webp");
        background-position: 10px center; 
        background-repeat: no-repeat;
        background-size: 20px 20px; 
        padding-left: 40px; 
        height: 40px; 
      }
      .sign-in-container {
      margin-top: 550px;
      margin-left: 40px;
      display: flex; 
      align-items: center; 
      justify-content: flex-start; 
      position: absolute; 
      left: 0; 
    }

    .sign-in-container p,
    .sign-in-container a {
    margin: 0; 
    padding: 0; 
    font-size: 14px;
    font-weight: bold;
    color: black;
    margin-right: 5px; 
    }



      .action-group input[type="text"] {
        height: 30px;

        padding: 12px;
        font-size: 16px;
        border: 1px solid #ddd;
        flex: 6; 
      }

      .action-group select {
        height: 56px;
        padding: 12px;
        font-size: 16px;
        border: 1px solid #ddd;
        flex: 1; 
        cursor: pointer;
      }

      .search {
        height: 56px;
        width: 400px;
        padding: 12px;
        font-size: 18px;
        background-color: black;
        color: white;
        border: none;
        cursor: pointer;
        border-radius: 8px;
        flex: 1.5; 
      }

      
      .picture-section {
       
        
        display: flex;
        justify-content: flex-start; 
        padding: 80px 0px;
        background-color: white;
      }

      .picture-item {
        
        width: 100%; 
        height: 100%;
        text-align: center;
        margin-right: 20px; 
      }

      .picture-item img {
        
        width: 610px; 
        height: 340px; 
      }

      header {
        background-color: transparent;
        position: fixed;
        top: 0;
        width: 100%;
        height: 65px;
        z-index: 1000;
        transition: background-color 0.3s;
      }
      .cities-container {
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
      }

      .cities {
        margin-top: 50px;
        line-height: 44px;
        font-weight: 700;
        font-size: 36px;
        margin-left: 40px;
      }
      .viewall {
        line-height: 20px;
        font-weight: 500;
        cursor: pointer;
        font-size: 16px;

        color: black;
        margin-right: 40px;
      }

      .header-container {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px 20px;
        max-width: 100%;
        margin: 5px;
        background-color: transparent;
      }

      .header-left {
        display: flex;
        align-items: center;
        gap: 15px;
      }

      .menu-btn {
        cursor: pointer;
        color: black;
        background-color: transparent;
        border: none;
      }

      .logo a {
        font-size: 18px;
        font-weight: bold;
        color: black;
        text-decoration: none;
      }

      .address-button {
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: black;
        color: white;
        border: none;
        width: 222.06px;
        height: 36px;
        padding: 8px 15px;
        border-radius: 20px;
        gap: 8px;
        cursor: pointer;
        opacity: 0;
        transition: opacity 0.3s;
      }

      .header-right {
        display: flex;
        justify-content: flex-end;
        margin-right: 20px;
        gap: 15px;
      }

      .header-right button {
        font-size: 14px;
        background: none;
        border: none;
        cursor: pointer;
        color: black;
        
        padding: 10px 13px;
        border-radius: 25px;
      }

      .header-right .signup {
        background-color: black;
        color: white;
      }
      .header-right .login {
        background-color: white;
        color: black;
      }

      .header-right .signup:hover {
        background-color: #282828;
      }

      .header-right button:hover {
        background-color: #f3f3f3;
      }

      .sidebar {
        box-sizing: border-box;
        max-width: 80%;
        height: 100%;
        width: 300px;
        position: fixed;
        padding: 30px;
        top: 0;
        left: 0;
        background-color: white;
        overflow-y: auto;
        padding-top:50px;
        display: none;
        z-index: 2000;
      }
      .sidebar a {
        flex-direction: column;
        text-decoration: none;
        display: block;
        transition: 0.3s;
      }
      .loginbutton {
        text-align: center;
        color: black;
        font-size: 18px;
        margin-top: 10px;
    
       width: 256px;
        min-height: 50px;
       text-align: center;
        display: flex;
        background-color: #ddd;
        border-radius: 8px;
        line-height: 24px;
  }

.signupbutton {
  font-size: 18px;
  width: 256px;
  min-height: 56px;
  text-align: center;
  display: flex;
  color: white;
 
  padding: 0px 0px;
  background-color: black;
  border-radius: 8px;
  line-height: 24px;
}
.option{
  font-weight: normal;
  margin-top:20px;
  font-size: 14px;
  width: 252px;
  display: flex;
  color: black;
  background-color: white;
}

      .close-btn {
        position: absolute;
        top: 10px;
        right: 25px;
        font-size: 36px;
        color: black;
        text-decoration: none;
        cursor: pointer;
      }

      .scrolled-header {
        background-color: white;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      }

      .scrolled-header .address-button {
        opacity: 1;
      }
      #map {
        height: 360px;
        width: 1823px;
        margin-left: 40px;
        margin-top: 20px;
      }
      .city-grid {
        margin-top: 10px;
        margin-left: 20px;
        width: 100%;
        max-width: 1823px;
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: repeat(6, 1fr);
        gap: 16px;
        padding: 10px;
        grid-auto-flow: column;
        justify-items: start;
      }

      .city-grid a {
        text-decoration: none;
        color: black;
        font-size: 16px;
        display: block; 
        text-align: center;
        padding: 7px;
        border: 1px solid transparent;
      }
      .country-grid {
        margin-top: 10px;
        margin-left: 20px;
        width: 100%;
        max-width: 1823px;
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: repeat(8, 1fr);
        gap: 16px;
        padding: 10px;
        grid-auto-flow: column;
        justify-items: start;
      }

      .country-grid a {
        text-decoration: none;
        color: black;
        font-size: 16px;
        display: block; 
        text-align: center;
        padding: 7px;
        border: 1px solid transparent;
      }

      .coutry-container {
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
      }

      .country {
        margin-top: 50px;
        line-height: 44px;
        font-weight: 700;
        font-size: 36px;
        margin-left: 40px;
      }
      .viewallcountry {
        line-height: 20px;
        font-weight: 500;
        cursor: pointer;
        font-size: 16px;

        color: black;
        margin-right: 40px;
      }
    

   
      .footer {
        background-color: white;
        padding: 40px 20px;
        font-family: Arial, sans-serif;
        color: #333;
        font-size: 14px;
      }

      .footer-container {
        max-width: 1200px;
        margin: 0 auto;
      }

      
      .footer-row {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
      }

      .image {
        padding-bottom: 20px;
        margin-top: 30px;
        width: 600px;
        height: 264px;
        flex: 2;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
      }

      .app {
        
        justify-content: space-between;
        display: flex;
        margin-top: 200px; 
      }

      .app a {
        
        display: -webkit-flex;
        margin-right: 10px;
      }

      .gethelp,
      .nearme {
        margin-top: 20px;
        flex: 1;
      }

      .gethelp ul,
      .nearme ul {
        list-style: none;
        padding: 0;
      }

      .gethelp li,
      .nearme li {
        margin-bottom: 15px;
      }

      .gethelp a,
      .nearme a {
        color: black;
        margin-bottom: 16px;
        line-height: 24px;
        font-weight: normal;
        font-size: 16px;
        text-decoration: none;
      }

      .gethelp a:hover,
      .nearme a:hover {
        text-decoration: underline;
      }

   
      .space2 {
        margin: 20px 0;
        border: none;
        border-top: 1px solid #ddd;
      }

    
      .google {
        margin-bottom: 10px;
        font-size: 12px;
        color: #666;
      }

      .last {
        font-size: 12px;
        color: #666;
        text-align: center;
      }
      .space {
        width: 100%;
        height: 70px;
        background-color: white;
        border-bottom: 1px solid #ddd;
      }
      
      #select {
        padding-left: 30px; 
        background-image: url("./images/time.webp");
        background-position: 5px center; 
        background-repeat: no-repeat;
        background-size: 20px 20px; 
      }

      option.deliver-now {
        background-image: url("path/to/your/image.jpg");

        background-position: px center; 
        background-repeat: no-repeat;
        padding-left: 30px; 
      }
      .last {
        padding-top:  20px;
    display: flex;
    justify-content: space-between; 
    align-items: flex-start; 
    padding: 20px;
    background-color:white; 
  }

.social {
 
  margin: 0;
  width: 96px;
  display: flex;
  gap: 10px; 
}

.social img {
  margin: 0;
  width: 18px;
  height: 18px;
  padding: 5px;
}

.copyright {
 
  color: black;
  font-weight: normal;
  margin-bottom: 16px;
  line-height: 20px;
  font-size: 14px;
  display: flex;
  flex-direction: column;
  align-items: flex-end; 
  gap: 10px;
}

.copyright-links {
  display: flex; 
  gap: 30px; 
}

.copyright-links a {
  color: black;
  text-decoration: none;
}

.copyright-links a:hover {
  
  text-decoration: underline;
}
.Inc {
  display: flex; 
  gap: 15px; 
  color: black;
  font-size: 14px;
  margin-top: 10px;
  align-items: flex-end;
  line-height: 20px;
  font-weight: normal;
}



    </style>
  </head>
  <body>
    <div id="sidebar" class="sidebar">
      <a href="#" class="close-btn" onclick="toggleSidebar()">×</a>
      <a href="#" class="signupbutton">Sign up</a>
      <a href="#" class="loginbutton">Log in</a>
      <a href="#" class="option">Create a business account</a>
      <a href="#"class="option">Add your restaurant</a>
      <a href="#"class="option">Sign up to deliver</a>
    </div>

    <header id="header">
      <div class="header-container">
        <div class="header-left">
          <button class="menu-btn" onclick="toggleSidebar()">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none">
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M23 4H1v3h22V4Zm0 7H1v3h22v-3ZM1 18h22v3H1v-3Z"
                fill="currentColor"
              ></path>
            </svg>
          </button>
          <div class="logo">
            <a href="#">UberEats</a>
          </div>
          <button class="address-button" type="button">
            <img
              src="images/left-icon.png"
              alt="Left Icon"
              class="lefticon"
              width="20px"
              height="20px"
            />
            Enter delivery address
            <img
              src="images/right-icon.png"
              alt="Right Icon"
              class="righticon"
              width="10px"
              height="10px"
            />
          </button>
        </div>

        <div class="header-right">
          <button type="button" class="login">Log in</button>
          <button type="button" class="signup">Sign up</button>
        </div>
      </div>
    </header>

    <main>
      <div class="main-content">
        <h1>Order delivery near you</h1>
        <div class="action-group">
          <input
            type="text"
            placeholder="     Enter delivery address"
            class="input"
          />
          <select name="select" id="select">
            <option value="deliver now">Deliver Now</option>
            <option value="schedule for later">Schedule for Later</option>
          </select>
          <button type="button" class="search">Search here</button>
          
          
        </div>
      </div>
      <div class="sign-in-container">
        <p>Or</p>
        <a href="#" >Sign In</a>
    </main>

    </div>

    <div class="picture-section">
      <div class="picture-item">
        <a href="#">
          <img src="./images/picture1.webp" alt="Feed your employees" />
          <p class="sentence">Feed your employees</p>
          <p class="sentence1">Create a business account</p>
        </a>
      </div>
      <div class="picture-item">
        <a href="#">
          <img src="./images/picture2.webp" alt="Your restaurant, delivered" />
          <p class="sentence">Your restaurant,<br />delivered</p>
          <p class="sentence1">Add your restaurant</p>
        </a>
      </div>
      <div class="picture-item">
        <a href="#">
          <img src="./images/picture3.webp" alt="Deliver with UberEats" />
          <p class="sentence">Deliver with UberEats</p>
          <p class="sentence1">Sign up to deliver</p>
        </a>
      </div>
    </div>
    <div class="cities-container">
      <h2 class="cities">Cities near me</h2>
      <a class="viewall" href="#">View all500+ cities</a>
    </div>

    <div id="map"></div>
    <div class="city-grid">
      <a href="https://www.ubereats.com/akron" target="_blank">Akron</a>
      <a href="https://www.ubereats.com/albuquerque" target="_blank"
        >Albuquerque</a
      >
      <a href="https://www.ubereats.com/bridgeport" target="_blank"
        >Bridgeport</a
      >
      <a href="https://www.ubereats.com/concord" target="_blank">Concord</a>
      <a href="https://www.ubereats.com/dayton" target="_blank">Dayton</a>
      <a href="https://www.ubereats.com/el-paso" target="_blank">El Paso</a>
      <a href="https://www.ubereats.com/hartford" target="_blank">Hartford</a>
      <a href="https://www.ubereats.com/houston" target="_blank">Houston</a>
      <a href="https://www.ubereats.com/indianapolis" target="_blank"
        >Indianapolis</a
      >
      <a href="https://www.ubereats.com/mcallen" target="_blank">McAllen</a>
      <a href="https://www.ubereats.com/mesa" target="_blank">Mesa</a>
      <a href="https://www.ubereats.com/milwaukee" target="_blank">Milwaukee</a>
      <a href="https://www.ubereats.com/nashville" target="_blank">Nashville</a>
      <a href="https://www.ubereats.com/new-orleans" target="_blank"
        >New Orleans</a
      >
      <a href="https://www.ubereats.com/oklahoma-city" target="_blank"
        >Oklahoma City</a
      >
      <a href="https://www.ubereats.com/omaha" target="_blank">Omaha</a>
      <a href="https://www.ubereats.com/orlando" target="_blank">Orlando</a>
      <a href="https://www.ubereats.com/palm-bay" target="_blank">Palm Bay</a>
      <a href="https://www.ubereats.com/providence" target="_blank"
        >Providence</a
      >
      <a href="https://www.ubereats.com/queens" target="_blank">Queens</a>
      <a href="https://www.ubereats.com/san-antonio" target="_blank"
        >San Antonio</a
      >
      <a href="https://www.ubereats.com/stony-brook" target="_blank"
        >Stony Brook</a
      >
      <a href="https://www.ubereats.com/tucson" target="_blank">Tucson</a>
      <a href="https://www.ubereats.com/west-hollywood" target="_blank"
        >West Hollywood</a
      >
    </div>

    <div class="coutry-container">
      <h2 class="country">Countries with Uber Eats</h2>
      <a class="viewallcountry" href="#">View all countries</a>
    </div>
    <div class="country-grid">
      <a href="https://www.ubereats.com/australia" target="_blank">Australia</a>
      <a href="https://www.ubereats.com/belgium" target="_blank">Belgium</a>
      <a href="https://www.ubereats.com/canada" target="_blank">Canada</a>
      <a href="https://www.ubereats.com/chile" target="_blank">Chile</a>
      <a href="https://www.ubereats.com/costa-rica" target="_blank"
        >Costa Rica</a
      >
      <a href="https://www.ubereats.com/dominican-republic" target="_blank"
        >Dominican Republic</a
      >
      <a href="https://www.ubereats.com/ecuador" target="_blank">Ecuador</a>
      <a href="https://www.ubereats.com/el-salvador" target="_blank"
        >El Salvador</a
      >
      <a href="https://www.ubereats.com/france" target="_blank">France</a>
      <a href="https://www.ubereats.com/germany" target="_blank">Germany</a>
      <a href="https://www.ubereats.com/guatemala" target="_blank">Guatemala</a>
      <a href="https://www.ubereats.com/ireland" target="_blank">Ireland</a>
      <a href="https://www.ubereats.com/italy" target="_blank">Italy</a>
      <a href="https://www.ubereats.com/japan" target="_blank">Japan</a>
      <a href="https://www.ubereats.com/kenya" target="_blank">Kenya</a>
      <a href="https://www.ubereats.com/luxembourg" target="_blank"
        >Luxembourg</a
      >
      <a href="https://www.ubereats.com/mexico" target="_blank">Mexico</a>
      <a href="https://www.ubereats.com/netherlands" target="_blank"
        >Netherlands</a
      >
      <a href="https://www.ubereats.com/new-zealand" target="_blank"
        >New Zealand</a
      >
      <a href="https://www.ubereats.com/panama" target="_blank">Panama</a>
      <a href="https://www.ubereats.com/poland" target="_blank">Poland</a>
      <a href="https://www.ubereats.com/portugal" target="_blank">Portugal</a>
      <a href="https://www.ubereats.com/south-africa" target="_blank"
        >South Africa</a
      >
      <a href="https://www.ubereats.com/spain" target="_blank">Spain</a>
      <a href="https://www.ubereats.com/sri-lanka" target="_blank">Sri Lanka</a>
      <a href="https://www.ubereats.com/sweden" target="_blank">Sweden</a>
      <a href="https://www.ubereats.com/switzerland" target="_blank"
        >Switzerland</a
      >
      <a href="https://www.ubereats.com/taiwan" target="_blank">Taiwan (ROC)</a>
      <a href="https://www.ubereats.com/united-kingdom" target="_blank"
        >United Kingdom</a
      >
      <a href="https://www.ubereats.com/united-states" target="_blank"
        >United States</a
      >
    </div>
    <div class="space"></div>

    <footer id="footer" class="footer">
      <div class="footer-container">
      
        <div class="footer-row">
          <div class="image">
            <img
              src="./images/uber.svg"
              alt="Uber Eats logo"
              width="134"
              height="24"
              class="ubereats"
            />
            <div class="app">
              <a
                href="https://apps.apple.com/us/app/uber-eats-food-delivery/id1058959277"
              >
                <img
                  alt="Download on the App Store"
                  src="./images/apple.svg"
                  height="40"
                  width="135"
                  class="ef"
                />
              </a>
              <a
                href="https://play.google.com/store/apps/details?id=com.ubercab.eats"
              >
                <img
                  alt="Get it on Google Play"
                  src="./images/android.png"
                  height="40"
                  width="134"
                  class="ef"
                />
              </a>
            </div>
          </div>

          <div class="gethelp">
            <ul>
              <li><a href="//help.uber.com/ubereats">Get Help</a></li>
              <li><a href="//uber.com/gift-cards/">Buy gift cards</a></li>
              <li>
                <a href="//merchants.ubereats.com/s/signup/"
                  >Add your restaurant</a
                >
              </li>
              <li>
                <a href="//www.uber.com/drive/delivery/">Sign up to deliver</a>
              </li>
              <li>
                <a href="//www.uber.com/business/eats"
                  >Create a business account</a
                >
              </li>
              <li><a href="/promo">Promotions</a></li>
            </ul>
          </div>

          <div class="nearme">
            <ul>
              <li><a href="/near-me">Restaurants near me</a></li>
              <li><a href="/location">View all cities</a></li>
              <li><a href="/location#all-countries">View all countries</a></li>
              <li><a href="/pickup/near-me">Pickup near me</a></li>
              <li><a href="//about.ubereats.com">About Uber Eats</a></li>
              <li><a href="/shopping">Shop groceries</a></li>
              <li><a href="#">English</a></li>
            </ul>
          </div>
        </div>

        <hr class="space2" />
        <div class="last">
          <div class="social">
            <a href="#"><img src="./images/facebook.png" alt="Facebook"></a>
            <a href="#"><img src="./images/twitter.png" alt="Twitter"></a>
            <a href="#"><img src="./images/instagram.png" alt="Instagram"></a>
          </div>
          
          <div class="copyright">
            <div class="copyright-links">
              <a href="#">Privacy Policy</a>
              <a href="#">Terms</a>
              <a href="#">Pricing</a>
              <a href="#">Do Not Sell or Share My Personal Information</a>
            </div>
            
            <div class="Inc">
              <p>This site is protected by reCAPTCHA and the Google Privacy Policy and Terms of Service apply.</p>
              <p>© 2024 Uber Technologies Inc.</p>
            </div>
          </div>
        </div>
        

       
      
    </footer>

    <script>
      function initMap() {
       
        const bounds = {
          north: 49.384358,
          south: 24.396308,
          east: -66.93457,
          west: -125.0,
        };

     
        const map = new google.maps.Map(document.getElementById("map"), {
          zoom: 5, 
          center: { lat: 37.0902, lng: -95.7129 },
          restriction: {
            latLngBounds: bounds, 
            strictBounds: false, 
          },
        });

        
        const marker = new google.maps.Marker({
          position: { lat: 37.0902, lng: -95.7129 }, 
          map: map,
          title: "United States",
        });
      }
    </script>


    <script
      src="https://maps.googleapis.com/maps/api/js?AIzaSyDzPlOrrX0AKO9_rPcFimuY3HCW2UlaU0w&callback=initMap"
      async
      defer
    ></script>

    <script>
      function toggleSidebar() {
        const sidebar = document.getElementById("sidebar");
        sidebar.style.display =
          sidebar.style.display === "block" ? "none" : "block";
      }

      window.addEventListener("scroll", function () {
        const header = document.getElementById("header");
        if (window.scrollY > 50) {
          header.classList.add("scrolled-header");
        } else {
          header.classList.remove("scrolled-header");
        }
      });
    </script>
  </body>
</html>
