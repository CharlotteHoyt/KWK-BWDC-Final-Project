<script>
  import { onMount } from 'svelte';
    onMount(() => {
      var divElement = document.getElementById('viz1753141259368');                    
      var vizElement = divElement.getElementsByTagName('object')[0];                    
      vizElement.style.width='1244px';vizElement.style.height='727px';                    
      var scriptElement = document.createElement('script');                    
      scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
      vizElement.parentNode.insertBefore(scriptElement, vizElement);    
    });

  import LeftAlignedExample from "./sections/LeftAlignedExample.svelte";
  import RightAlignedExample from "./sections/RightAlignedExample.svelte";
  import ImageExample from "./sections/ImageExample.svelte";
  import TitleSection from "./sections/TitleSection.svelte";
  import InteresectionObserverBasicExample from "./sections/InteresectionObserverBasicExample.svelte";
  import IntersectionObserverAlertExample from "./sections/IntersectionObserverAlertExample.svelte";
  import DisappearingDuckExample from "./sections/DisappearingDuckExample.svelte";
  import IntersectionObserverSectionCard from "./sections/IntersectionObserverSectionCard.svelte";
  import IntersectionObserverListExample from "./sections/IntersectionObserverListExample.svelte";
</script>

<main>
  <TitleSection />
  <RightAlignedExample />
  <LeftAlignedExample />
  <!--<ImageExample />-->

  <!--<IntersectionObserverSectionCard />
  <InteresectionObserverBasicExample />
  <IntersectionObserverAlertExample />
  <DisappearingDuckExample />
  <IntersectionObserverListExample />-->

  <h1 class="center">Check Out the Visualization!</h1>
  <br>
  
  <div class='tableauPlaceholder' id='viz1753141259368' style='position: relative'>
    <noscript>
      <a href='#'>
        <img alt='Map: Internet Subscriptions ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;BW&#47;BWDC-EducationEmployment-InternetSubscriptions&#47;MapInternetSubscriptions&#47;1_rss.png' style='border: none' />
      </a>
    </noscript>
    <object class='tableauViz'  style='display:none;'>
      <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> 
      <param name='embed_code_version' value='3' /> 
      <param name='site_root' value='' />
      <param name='name' value='BWDC-EducationEmployment-InternetSubscriptions&#47;MapInternetSubscriptions' />
      <param name='tabs' value='no' />
      <param name='toolbar' value='yes' />
      <param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;BW&#47;BWDC-EducationEmployment-InternetSubscriptions&#47;MapInternetSubscriptions&#47;1.png' /> 
      <param name='animate_transition' value='yes' />
      <param name='display_static_image' value='yes' />
      <param name='display_spinner' value='yes' />
      <param name='display_overlay' value='yes' />
      <param name='display_count' value='yes' />
      <param name='language' value='en-US' />
      <param name='origin' value='viz_share_link' />
      <param name='filter' value='padding=0' />
      <param name='filter' value='position=relative' />
    </object>
  </div>

  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>

  <div class="section">
    <h1>Community Connections</h1>
    <p>My county, King County (in Washington state), recognizes broadband as an "essential utility" and has conducted an access study to expand broadband infrastructure and make high speed internet more affordable for King County residents.</p>
    <p>This survey explores the access and availability of broadband. The report both recognizes obstacles and proposes solutions related to high speed internet access and internet affordability.</p>
    <p>This is an excellent example of a county making an effort to accomplish digital equity.</p>

    <br>
    <br>

    <div class="content">
        <strong class="articleTextHeader">Check Out the Report!</strong>
        <p class="articleTextCaption">Read King County's <a href="https://kingcounty.gov/en/dept/kcit/data-information-services/broadband" target="_blank">broadband internet access survey</a> on the county's official website.</p>
    </div>
  </div>

  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>

  <div class="section">
    <h1>Conclusions</h1>
    <p>Broadband is crucial for modern life in the United States and is fundamental for healthcare, education, economic development, job searching, and general social connectivity.</p>
    <p>Digital redlining and internet access disparities are a major issue. Denying or limiting broadband access to certain areas or populations creates an exclusive digital landscape. Combatting discrimination in the provision of internet service and access starts with advocacy, efforts to expand infrastructure, and the promotion of digital literacy.</p>

    <br>
    <br>

    <div class="content">
        <strong class="articleTextHeader">How to Help</strong>
        <ul>
          <li class="bulletPoint">Build public awareness about digital redlining.</li>
          <li class="bulletPoint">Support legislation promoting digital equity and engage with policymakers.</li>
          <li class="bulletPoint">Stay educated on the problem! Strive to understand the interconnected issues that shape it.</li>
        </ul>
    </div>
  </div>

  <br>
  <br>
</main>

<style>
  .section {
    width: 90%;
    margin-right: auto;
    margin-left: auto;
  }

  h1 {
    font-size: 3rem;
    margin: 0;
    color: #DDA853;
    font-family: "Contrail One", sans-serif;
    margin-bottom: -.25em;
  }

  p {
    font-size: 1.3rem;
    color: #F3F3E0;
    margin-top: 1rem;
    font-family: "Inclusive Sans", sans-serif;
    font-weight: 500;
  }

  a {
    color: #DDA853;
  }

  .content {
    margin-right: auto;
    margin-left: auto;
    max-width: 700px;
    background-color: #27548A;
    padding: 2rem;
    border: 6px solid #DDA853;
    box-shadow: 16px 16px #183B4E;
  }

  .articleTextHeader {
    color: #DDA853;
    font-family: "Contrail One", sans-serif;
    font-size: 1.7rem;
  }

  .articleTextCaption {
    margin-top: 0em;
  }

  .bulletPoint {
    font-size: 1.3rem;
    color: #F3F3E0;
    margin-top: 1rem;
    font-family: "Inclusive Sans", sans-serif;
    font-weight: 500;
  }

  .tableauPlaceholder {
    width: 50%;
    margin-right: auto;
    margin-left: auto;
    display: block;
    border: 6px solid #DDA853;
    box-shadow: 16px 16px #183B4E;
 }

  .center {
    text-align: center;
  }
</style>
