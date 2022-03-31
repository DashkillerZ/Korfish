<script></script>
<div class="main">
    <div>
        <h1>
            Pricing
        </h1>
        <h4>Website Security Platform Plans</h4>
        <div class="grid">
            <div>
                <h3>1 Month</h3>
                <h2>USD&dollar; 49/MO</h2>
                <!-- <h4 class="offer">USD&dollar; 49/MO</h4> -->
                <!-- <h4>15&percnt; off</h4> -->
            </div>
            <div>
                <span>Reccomanded</span>
                <h3>12 Month</h3>
                <h2>USD&dollar; 41/MO</h2>
                <h4 class="offer">USD&dollar; 49/MO</h4>
                <h4>15&percnt; off</h4>
            </div>
            <div>
                <h3>24 Month</h3>
                <h2>USD&dollar; 36/MO</h2>
                <h4 class="offer">USD&dollar; 49/MO</h4>
                <h4>25&percnt; off</h4>
            </div>
            <div>
                <h3>36 Month</h3>
                <h2>USD&dollar; 24/MO</h2>
                <h4 class="offer">USD&dollar; 49/MO</h4>
                <h4>50&percnt; off</h4>
            </div>
        </div>
    </div>
    <div>
        <h1>Quick Response &amp; alert of <span>HACKING ATTEMPTS</span></h1>
        <div class="flex">
            <img src="./assets/img/Group62.png" alt="">
            <div>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iusto exercitationem quidem voluptas reprehenderit deserunt? Corporis fugit voluptate dicta nisi iste sequi, impedit, velit molestias voluptas nulla ratione fugiat! Ducimus fugiat animi adipisci harum, iure maiores nihil libero quaerat. Quasi quaerat eius animi iure vero nisi ea dolores, odit mollitia nostrum! Repellendus officiis inventore optio ea enim fuga exercitationem soluta dolore.
            </div>
        </div>
    </div>
</div>
    
<style>
    /* ----------------------------------------------------------------------*/
    .main >*{
        padding: 50px 6vw;
    }
    .main div:first-child>h1{
        color: #E81C25;
        margin: 0;
    }
    .main div:first-child>h4{
        margin: 0;
        color: #525252;
    }
    .main .grid{
        padding: 50px 0;
        display: grid;
        grid-template-columns: repeat(auto-fit,280px);
        justify-content: center;
        
    }
    .main .grid >div{
        border: 3px solid #ddd;
        margin: 10px auto;
        width: 220px;
        height:185px;
        text-align: center;
        border-radius: 15px;
    }

    .main .grid >div span{
        position: absolute;
        width: 150px;
        font-size: 0.85rem;
        height: 25px;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 25px;
        color:white;
        background: #0BBC2A;
        transform: translate(35px,-15px);
    }
    .main .grid >div h4{
        margin: 5px 0 0 0;
    }
    .main .grid >div .offer{
        text-decoration: line-through;
        color: #E81C25;
        padding: 0;
        margin: 10px 0 0 0;
    }
    
    .main div:last-child h1 span{
        color: #E81C25;
        text-decoration: underline;
    }
    .main div:last-child .flex{
        display: flex;
        justify-content: center;
        align-items: center;
        color: #525252;
        font-weight: 500;
    }
    .main div:last-child .flex img{
        margin: 0 20px 0 0;
    }
    
    /* ----------------------------------------------------------------------*/
    @media (max-width:830px){
        .main div:last-child .flex{
            text-align: justify;
        }  
        .main div:last-child .flex img{
            display: none;
        }  
    }
</style>