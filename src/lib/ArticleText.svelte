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
        width: 65%;
        background-color: #27548A;
        color: #F3F3E0;
        border: solid #DDA853 4px;
        padding: 20px;
        box-shadow: 10px 10px #183B4E;
        font-weight: 500;
        font-size: 1.3rem;
    }
</style>
