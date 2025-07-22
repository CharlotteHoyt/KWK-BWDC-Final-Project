<script>
    let { title, subtitle } = $props();
</script>

<div class="title-card">
    <div class="content">
        <h1>{title}</h1>
        <p>{subtitle}</p>
    </div>
</div>

<style>
    .title-card {
        background-color: #27548A;
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        padding: 2rem;
        box-sizing: border-box;
    }

    .content {
        max-width: 700px;
        background-color: #27548A;
        padding: 2rem;
        border: 6px solid #DDA853;
        box-shadow: 16px 16px #183B4E;
    }

    h1 {
        font-size: 3rem;
        margin: 0;
        color: #DDA853;
        font-family: "Contrail One", sans-serif;
    }

    p {
        font-size: 1.3rem;
        color: #F3F3E0;
        margin-top: 1rem;
        font-family: "Inclusive Sans", sans-serif;
        font-weight: 500;
    }

    @media (max-width: 600px) {
        h1 {
            font-size: 2.2rem;
        }

        p {
            font-size: 1.1rem;
        }
    }
</style>
