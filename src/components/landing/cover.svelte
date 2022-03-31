
<script>
    particlesJS.load('particles-js', './assets/custom/particles.json', function() {
        console.log('callback - particles.js config loaded');
    });
</script>
<div class="main">
    <div class="wrap">
        <div>
            Web Security Made Simple  
        </div>
        <div>
            Protect Websites From Hacks And Attacks
        </div>
        <div class="tags">
            <span>Bad Bots</span>
            <span>Bad Words</span>
            <span>Proxy Protection</span>
            <span>Spam Protection</span>
            <span>SQLi Protection</span>
        </div>
        <div class="btn">
            <img src="./assets/img/Group11.png" alt="" />
            <span>&nbsp;See&nbsp;Plans&nbsp;And&nbsp;Features</span>
        </div>
    </div>
    <div id="particles-js"></div>
</div>
<style>
    .main{
        display: grid;
        background: #000;
        height: 500px;
        overflow: hidden;
        grid-template-columns: 1fr 1fr;
    }
    #particles-js{
        height: 500px;
        margin-left: auto;
        width: 40vw;
    }
    .wrap{
        height: 500px;
        background: linear-gradient(to right,#323232 60%,transparent);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
        padding:0 0 0 6vw;
        margin: 0 !important;
        /* overflow: hidden; */
        color: white;
    }
    .main div:first-child{
        font-size: 1.2rem;
        font-weight: 500;
        margin:10px 0;
        
    }
    .main div:nth-child(2){
        font-size: 2rem;
        margin:10px 0;
        padding: 0;
        
    }
    .tags{
        margin:10px 0;

    }
    .tags span{
        border-right: 2px solid #E81C25;
        padding: 0 5px ;
    }
    .tags span:last-child{
        border-right: none;
    }
    .btn{
        margin:20px 0;
        background: #E81C25;
        height: 30px;
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 5px 10px;
        border-radius:40px;
    }
    @media (max-width:830px){
        .main{
            display: grid;
            height: unset;
            grid-template-areas:
            "particle"
            "wrap";
        }
        .wrap{
            grid-area:wrap ;
            height:400px;
            overflow: hidden;
            background: linear-gradient(to top,#242424 60%,transparent);
        }
        #particles-js{
            grid-area: particle;
            width: 100vw;
            height: 300px;
        }
    }
</style>