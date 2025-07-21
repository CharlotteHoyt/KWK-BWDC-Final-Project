<script>
    let { children } = $props();
</script>

<div class="article-text">
    <p>
        {@render children()}
    </p>
</div>

<style>
    .article-text {
        margin: 50vh auto;
        /*width: 50%;*/
        width: 65%;
        /*background-color: #ff99fc;*/
        background-color: #27548A;
        /*color: #007052;*/
        color: #F3F3E0;
        /*border: solid #8427c9 3px;*/
        border: solid #DDA853 4px;
        /*border-radius: 20px;*/
        padding: 20px;
        /*box-shadow: 16px 16px #8aa6df;*/
        box-shadow: 10px 10px #183B4E;

        font-weight: 500;
        font-size: 1.3rem;
    }
</style>
