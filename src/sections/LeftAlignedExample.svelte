<script>
    import * as Highcharts from "highcharts";
    import "highcharts/modules/exporting";
    import { Chart } from "@highcharts/svelte";
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";

    const series = [
        {
            name: "Group 1",
            data: [
                [1990, 3],
                [2000, 4],
                [2010, 1],
                [2020, 1],
            ],
            color: "#8427c9",
        },
        {
            name: "Group 2",
            data: [
                [1990, 2],
                [2000, 5],
                [2010, -2],
                [2020, 2],
            ],
            color: "#ff99fc",
        },
        {
            name: "Group 3",
            data: [
                [1990, 4],
                [2000, 3],
                [2010, 0],
                [2020, 3],
            ],
            color: "#4096fa",
        },
    ];

    let chart;
    let thirdSeriesVisible = false;

    let options = {
        chart: {
            type: "spline",
            backgroundColor: "#e3ff00",
            borderColor: "#007052",
            borderWidth: 5,
            borderRadius: 20,
        },
        title: {
            text: "Another Example Chart",
        },
        subtitle: {
            text: "With a subtitle! And styling!",
        },
        series: [series[0], series[1]],
    };

    function toggleThirdSeries() {
        const existingSeries = chart.series.find((s) => s.name === "Group 3");

        if (existingSeries) {
            existingSeries.remove();
            thirdSeriesVisible = false;
        } else {
            chart.addSeries(series[2]);
            thirdSeriesVisible = true;
        }
    }
</script>

<div>
    <Scroller layout="left">
        {#snippet sticky()}
            <!--<div class="chart">
                <Chart bind:chart {options} highcharts={Highcharts} />
            </div>
            <button on:click={toggleThirdSeries} class="toggle-button">
                {thirdSeriesVisible ? "Remove Group 3" : "Add Group 3"}
            </button>-->
            <div>
                <h1>What the Data Reveals</h1>
                <p>Digital redlining is incredibly harmful and perpetuates inequities.</p>
                <p>Racial disparities exist in broadband access, limiting opportunity and hindering access.</p>
                <p>I looked into the issue of race and broadband internet access by exploring data and visualizations from the <a href="https://blackwealthdata.org" target="_blank">Black Wealth Data Center</a>, and I invite you to do the same! To the side, I have shared some of my discoveries!</p>
            </div>
        {/snippet}

        {#snippet scrolly()}
            <ArticleText>
                <strong class="articleTextHeader">Key Takeaway 1</strong>
                <p class="articleTextCaption">The three counties with the highest Black population percentages (Claiborne County, Holmes County, and Greene County) are also all in the bottom 25% of geographies as it pertains to the percentage of households with broadband internet access.</p>
            </ArticleText>

            <ArticleText>
                <strong class="articleTextHeader">Key Takeaway 2</strong>
                <p class="articleTextCaption">The southeastern United States, which has a large and historically significant Black population compared to other regions, has many counties with a lower percentage of households with broadband internet access.</p>
            </ArticleText>

            <ArticleText>
                <strong class="articleTextHeader">Key Takeaway 3</strong>
                <p class="articleTextCaption">Many localities in Mississipi and Alabama with Black populations over 70% lack access to broadband.</p>
            </ArticleText>

            <ArticleText>
                <strong class="articleTextHeader">Key Takeaway 4</strong>
                <p class="articleTextCaption">Cities and more populated regions generally have better access to/higher avalibility of broadband than rural areas.</p>
            </ArticleText>
        {/snippet}
    </Scroller>
</div>

<style>
    .chart {
        width: 90%;
        margin: 0px auto;
    }

    .toggle-button {
        margin: 20px;
        padding: 20px;
        color: #007052;
        background-color: #0bd956;
        border: solid 2px #007052;
        border-radius: 16px;
        font-size: large;
        cursor: pointer;
        transition: all 0.2s ease;
        box-shadow: 0 4px 0 #007052;
    }

    .toggle-button:active {
        transform: translateY(2px);
        box-shadow: 0 2px 0 #007052;
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
</style>
