<script>
    import ListItem from './listItem.svelte';

    import {onMount} from 'svelte';
    let header = [];
    onMount(async()=>{
        const response = await fetch('https://dashkiller.pythonanywhere.com/proxyprotection');
        header = await response.json();
    })  

    let posts = [];
    onMount(async()=>{
        const response = await fetch('https://dashkiller.pythonanywhere.com/proxyprotectionlist');
        posts = await response.json();
    })  

</script>
<div class="main">
    {#each header as item(item.id)}
        <div class="title">{item.title}</div>
        <div class="desc">{item.desc}</div>
        <div class="subtitle">{item.subtitle}</div>
        <div class="subdesc">{item.subdesc}</div>
    {/each}

    <div class="other">
        <div class="span"><i class="fas fa-umbrella"></i>&nbsp;Other Protection Options</div>
        <div class="list">
            {#each posts as post(post.id)}
                <ListItem title="{post.title}" desc="{post.desc}" summary="{post.summary}"/>
                {:else}
                <div>loading...</div>
            {/each}
        </div>
    </div>

</div>
<style>
    .main{
        padding: 50px 6vw;
    }
    .title{
        font-size: 1.5rem;
        margin: 0px 0 5px 0;
        text-transform: uppercase;
        text-shadow: 0 0 black;
    }
    .desc{
        font-size: 0.8rem;
        margin:0 0 25px 0;
        text-transform: uppercase;
    }
    .subtitle{
        font-size: 1.1rem;
        color: #0E406A;
        font-weight: 700;
        margin: 25px 0 5px 0;
    }
    .subdesc{
        font-size: 0.8rem;
        margin:0 0 25px 0;
    }
    .other{
        border: 1px solid #bbb;
        border-radius: 5px;
        padding-bottom: 15px;
    }
    .other .span{
        background: #0E406A;
        width: 260px;
        color: white;
        font-size: 1.2rem;
        border-bottom-right-radius: 15px;
        display: flex;
        align-items: center;
        justify-content: center;
        height: 50px;
        margin: 0 0 15px 0;
    }
    .list {
        padding: 0 15px ;
    }
    @media (max-width:480px){
        .other .span{
            width: 95%;
            border-bottom-right-radius: 15px;
            border-bottom-left-radius: 15px;
            justify-content: start;
            padding-left:5%;

        }
    }
</style>
