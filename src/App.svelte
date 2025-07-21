<script>
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
    /*margin-top: -300px;*/
    margin-right: auto;
    margin-left: auto;
  }

  h1 {
    font-size: 3rem;
    margin: 0;
    color: #DDA853;
    /*text-shadow: 1px 1px 0 #007052;*/

    font-family: "Contrail One", sans-serif;
    margin-bottom: -.25em;
  }

  p {
    font-size: 1.3rem;
    color: #F3F3E0;
    margin-top: 1rem;

    /*font-family: "Inter Tight", sans-serif;*/
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
    /*border-radius: 2rem;*/
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

    /*font-family: "Inter Tight", sans-serif;*/
    font-family: "Inclusive Sans", sans-serif;

    font-weight: 500;
  }
</style>
