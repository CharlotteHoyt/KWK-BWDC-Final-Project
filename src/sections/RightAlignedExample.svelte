<script>
    import * as Highcharts from "highcharts";
    import "highcharts/modules/exporting";
    import { Chart } from "@highcharts/svelte";
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";

    let options = {
        chart: {
            type: "pie",
        },
        title: {
            text: "An Example Pie Chart",
        },
        plotOptions: {
            pie: {
                allowPointSelect: true,
                dataLabels: [
                    {
                        enabled: true,
                        distance: 20,
                    },
                    {
                        enabled: true,
                        distance: -40,
                        format: "{point.percentage:.1f}%",
                        style: {
                            fontSize: "1.2em",
                            textOutline: "none",
                        },
                        filter: {
                            operator: ">",
                            property: "percentage",
                            value: 10,
                        },
                    },
                ],
            },
        },
        series: [
            {
                name: "Group",
                data: [
                    {
                        name: "Group 1",
                        y: 151,
                    },
                    {
                        name: "Group 2",
                        sliced: true,
                        selected: true,
                        y: 180,
                    },
                    {
                        name: "Group 3",
                        y: 32,
                    },
                    {
                        name: "Group 4",
                        y: 103,
                    },
                    {
                        name: "Group 5",
                        y: 77,
                    },
                ],
            },
        ],
    };
</script>

<div>
    <Scroller layout="right">
        {#snippet sticky()}
            <!--<div class="chart">
                <Chart {options} highcharts={Highcharts} />
            </div>
            <p>
                Here's an example chart using
                <a href="https://www.highcharts.com/">Highcharts</a>!
            </p>-->
            <h1>Importance of Broadband Internet</h1>
            <p>Broadband (short for "broad bandwidth") provides high-speed internet access and is extremely important for modern life.</p>
            <p>In today's world, broadband is no longer seen as a luxury. Many consider broadband a basic, essential service comparable to water and electricity.</p>
            <p>Broadband is vitally important for full participation in the digital age. In the United States, there is not universal access to broadband, fueling a digital divide.</p>
            <p>Learn more about the necessity of broadband internet by scrolling down the page.</p>
        {/snippet}

        {#snippet scrolly()}
            <ArticleText>
                <img class="scrollerBoxImage" src="healthcare.jpg" alt="Hands with red nails type at a laptop beside a blue stethoscope.">
                <p class="imageCaption">Image From <a href="https://unsplash.com/photos/person-sitting-while-using-laptop-computer-and-green-stethoscope-near-NFvdKIhxYlU" target="_blank">National Cancer Institute</a> on Unsplash</p>
                <br>
                <strong class="articleTextHeader">Healthcare</strong>
                <p class="articleTextCaption">Lack of broadband can also limit access to healthcare, health information, and telemedicine or make it difficult to connect with providers.</p>
            </ArticleText>

            <ArticleText>
                <img class="scrollerBoxImage" src="money.jpg" alt="United States one dollar bills folded and showing various sides on a flat off white surface.">
                <p class="imageCaption">Image From <a href="https://unsplash.com/photos/1-us-dollar-bill-_GNVwZJv-Jo" target="_blank">Emilio Takas</a> on Unsplash</p> 
                <br>
                <strong class="articleTextHeader">Wealth/Economy</strong>
                <p class="articleTextCaption">Broadband internet allows for remote work, e-commerce, entrepreneurship, and response to economic opportunities.</p>
            </ArticleText>

            <ArticleText>
                <img class="scrollerBoxImage" src="library.jpg" alt="A woman with brown hair and glasses reading a book against a colorful bookshelf.">
                <p class="imageCaption">Image From <a href="https://unsplash.com/photos/woman-reading-book-kcT-7cirBEw" target="_blank">Elliot Reyna</a> on Unsplash</p>
                <br>
                <strong class="articleTextHeader">Education</strong>
                <p class="articleTextCaption">Broadband access is essential for modern education, determining access to online materials, collaboration, participation in virtual classrooms, and opportunities for independent/extracurricular study.</p>
            </ArticleText>

            <ArticleText>
                <img class="scrollerBoxImage" src="interview.jpg" alt="Two women in conversation sitting across from each other in green chairs at a white table.">
                <p class="imageCaption">Image From <a href="https://unsplash.com/photos/two-women-sitting-beside-table-and-talking-LQ1t-8Ms5PY" target="_blank">Christina</a> on Unsplash</p>
                <br>
                <strong class="articleTextHeader">Job Seekers</strong>
                <p class="articleTextCaption">Increasingly important in job searching, access to broadband can determine the use of online job boards and networking platforms. Additionally, broadband access impacts participation in virtual interviews and remote work opportunities.</p>
            </ArticleText>

            <ArticleText>
                <img class="scrollerBoxImage" src="friends.jpg" alt="Many hands stacked together, some with rings others with painted nails. All arms have colorful sweaters.">
                <p class="imageCaption">Image From <a href="https://unsplash.com/photos/person-in-red-sweater-holding-babys-hand-Zyx1bK9mqmA" target="_blank">Hannah Busing</a> on Unsplash</p>
                <br>
                <strong class="articleTextHeader">Social Connectivity</strong>
                <p class="articleTextCaption">Broadband allows for engagement with online communities and social networks. Access to broadband can even open the door for civic engagement and discourse, while also simplifying access to government services.</p>
            </ArticleText>
        {/snippet}
    </Scroller>
</div>

<style>
    .chart {
        width: 90%;
        margin: 0px auto;
    }

    p {
        color: #F3F3E0;
        font-family: "Inclusive Sans", sans-serif;
        font-weight: 500;

        font-size: 1.3rem;
    }

     a {
        color: #DDA853;
     }

     h1 {
        color: #DDA853;
        font-size: 3em;
        font-family: "Contrail One", sans-serif;
        margin-bottom: -.25em;
     }

     .articleTextHeader {
        color: #DDA853;
        font-family: "Contrail One", sans-serif;
        font-size: 1.7rem;
     }

     .articleTextCaption {
        margin-top: 0em;
     }

     .scrollerBoxImage {
        height: 200px;
        margin: auto;
        display: block;
     }

     .imageCaption {
        font-size: .8em;
        text-align: center;
     }
</style>
