<script>

</script>
 <div class="main">
    <div>
        <h1>WHY KORFISH</h1>
        <div>Built For all Platforms & Websites</div>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Fugiat accusantium optio consequuntur, vero eveniet nulla consequatur repudiandae fuga amet delectus Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, consectetur? Dolores nostrum nulla cupiditate quam aliquam minima autem corrupti facere.</p>
    </div>
    <div>
        <div class="grid">
            <div>
                <div><i class="fas fa-database"></i> SQL Injection</div>
                <div>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Unde provident nostrum alias recusandae libero quis itaque nulla enim dignissimos minus.</div>
                <div>Read More <span><i class="fas fa-chevron-circle-right"></i></span></div>
            </div>
            <div>
                <div><i class="fab fa-edge"></i> SQL Injection</div>
                <div>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Unde provident nostrum alias recusandae libero quis itaque nulla enim dignissimos minus.</div>
                <div>Read More <span><i class="fas fa-chevron-circle-right"></i></span></div>
            </div>
            <div>
                <div><i class="fas fa-envelope"></i> SQL Injection</div>
                <div>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Unde provident nostrum alias recusandae libero quis itaque nulla enim dignissimos minus.</div>
                <div>Read More <span><i class="fas fa-chevron-circle-right"></i></span></div>
            </div>
            <div>
                <div><i class="fas fa-robot"></i> SQL Injection</div>
                <div>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Unde provident nostrum alias recusandae libero quis itaque nulla enim dignissimos minus.</div>
                <div>Read More <span><i class="fas fa-chevron-circle-right"></i></span></div>
            </div>
        </div>
        <div class="flex">
            <span>FEATURES</span>
            <span></span>
        </div>
    </div>
    <div>
        <div class="img">
            <img src="./assets/img/Group61.png" alt="" >
        </div>
        <h2>
            Simple And Hastle Free Steps to add Website
        </h2>
        <div>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptates at dolores deleniti sequi sapiente eum quo rerum minima molestias! Praesentium dolores, fugiat repellendus illo itaque aliquam natus minima iusto cum.
        </div>
        <ul>
            <li>
                Choose Plan & Combination of freatures
            </li>
            <li>
                Add a piece of code into your website
            </li>
            <li>
                That's it,You are secured now.
            </li>
        </ul>
        <div class="btn">
            <i class="far fa-edit"></i> Choose A Plan Now
        </div>
    </div>
  
    
</div>
 <style>
    .main > *{
        padding: 5px 6vw ;
        overflow: hidden;

     }
    /* ----------------------------------------------------------------------*/

    .main>div:first-child {
        margin: 20px 0 ;
    }
    .main>div:first-child h1{
        color: #E81C25;   
        margin: 15px 0 5px 0;
    }
    .main>div:first-child>div{
        color: #494949;
        font-weight: 500;
        font-size: 1.1em;
    }
    .main>div:first-child>div::after{
        content: "";
        display: block;
        width: 50px;
        margin-top: 10px;
        height: 2px;
        background: #E81C25;
    }
    .main>div:first-child>div{
        color: #494949;
        font-weight: 500;
        font-size: 1.1em;
    }
    .main>div:nth-child(2){
        background: #F2F2F2;
    }
    .main>div>.flex{
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
        font-size: 4rem;

    }
    .main>div>.flex span:first-child{
        margin: 0 10px;
        font-weight: 700;
        color: #ddd;
        transform: translateY(20px);
    }
    .main>div>.flex span:last-child{
        background: #E81C25;
        transform: translateY(4px);
        width:100%;
        height:1px;
        display: inline-block;
    }
    /* ----------------------------------------------------------------------*/

    .grid{
        display: grid;
        grid-template-columns: 1fr 1fr;
        margin: 60px 0 20px 0;
        
    }
    .grid>div{
        padding: 20px ;
        border-collapse: collapse;
    }
    .grid>div:first-child{
        border-right: 1px solid #ddd;
        border-bottom: 1px solid #ddd;
    }
    .grid>div:last-child{
        border-left: 1px solid #ddd;
        border-top: 1px solid #ddd;
        transform: translate(-1px,-1px);
    }
    .grid >div>div:first-child{
        font-weight: 700;
        display: flex;
        align-items: center;
        /* background: #000; */
        font-size: 1.2rem;
        margin: 10px 0;
    }
    .grid >div>div:first-child i{
        font-size: 2.2rem;
        color: #E81C25;
        margin: 0 10px 0 0;
    }
    .grid >div>div:last-child {
        color: #E81C25;
    }
    /* ----------------------------------------------------------------------*/
    .main>div:nth-child(3){
        display: grid;
        padding-block: 50px;
        grid-template-columns: 1fr 1fr;
    }
    .main>div:nth-child(3)>*{
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .main>div:nth-child(3) .img{
        grid-column: 2/3;
        grid-row:1/6 ;
        margin: 0 auto;
    }
    .main>div:nth-child(3)>h2{
        grid-column: 1/2;
        grid-row:2/3 ;
        color: #3b3b3b;
        display: block;
        
    }
    .main>div:nth-child(3) div:nth-child(3){
        grid-column: 1/2;
        grid-row:3/4 ;
        color: #525252;
    }
    .main>div:nth-child(3) ul{
        grid-column: 1/2;
        grid-row:4/5 ;
        flex-direction: column;
        align-items: flex-start;
        font-size: 1.1rem;
        font-weight: 500;
        color: #494949;
        list-style: "- ";
        padding: 0 10px;
    }
    .main>div:nth-child(3) .btn{
        grid-column: 1/2;
        grid-row:5/6 ;
        color: white;
        height: 30px;
        border-radius: 30px;
        padding: 5px 15px;
        background: #E81C25;
        width: max-content;
    }
    @media (max-width:830px){
        .grid{
            display: grid;
            grid-template-columns: 1fr;
            margin: 65px 0vw;
        }
        .grid>div{
            border: none ;
            border-bottom: 1px solid #ddd;
        }
        .grid>div:first-child{
            border-right: none;
        }
        .grid>div:last-child{
            border-left: none;
            border-top:none;
            border-bottom: none;
        }
        .main>div:nth-child(3){
            grid-template-columns: 1fr;
        }
        .main>div:nth-child(3) .img{
            display: none;
        }
        .main>div:nth-child(3) .btn{
            grid-column: 1/2;
            grid-row:5/6 ;
            margin: 0 auto;
        }
    }
 </style>