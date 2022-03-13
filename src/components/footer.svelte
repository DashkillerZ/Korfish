<script>
    
</script>
<div class="main">
    <div class="hl"></div>	
    <div class="grid"> 
        <div class="div1">
            <h2>+1&nbsp;937&nbsp;344&nbsp;6241</h2>
            <div>4031 Colonal Glenn Hwy Ste 100<br>Beavercreek, OH 45431</div>
            <div>&#169&nbsp;2022&nbsp;KORFISH</div>
        </div>
        <div class="div2">
            <div>
                <a href="">About</a>
                <a href="">Blog</a>
                <a href="">Contacts</a>
            </div>
            
            <div>
                <a href="">Admin&nbsp;Login</a>
                <a href="">Reseller&nbsp;Login</a>
                <a href="">Client&nbsp;Login</a>
            </div>
            <div>
                <a href="">Module&nbsp;&amp;&nbsp;Features</a>
                <a href="">Pricing</a>
                <a href="">Help&nbsp;Center</a>
            </div>
        </div>
        <div class="div3">
            <span class="vl"></span>
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-linkedin"></i></a>
            <a href="#"><i class="fab fa-youtube"></i></a>
        </div>
    </div>
</div>
<style>
    .main{
        height: auto;
        background-color: #F3F7FA;
        color: black;
        padding: 20px 0;
    }
    .grid{
        display: grid;
        grid-template-columns: 3fr 2fr 1fr;

    }
    .div1{
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-top: 13px;
    }
    .div1>h2{
        color: #5883af;
        font-size: 1.5rem;
        font-weight: bold;
        margin: 0;
    }
    .div2{
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        padding: 0 10px;
    }
    .div2 >div{
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 10px 0;
    }
    .div2 a{
        color: #5883af;
        text-decoration: none;
        padding: 8px 10px;
        font-weight: 500;
    }
    .div3{
        display: flex;
        border-left: 1px solid #5883af;
        justify-content: center;
        align-items: center;
    }
    .div3 >a{
        color: #000000;
        text-decoration: none;
        padding:0 8px;
    }
    @media (max-width:830px){
        .grid{
            grid-template-columns: 1fr;
        }
        .grid >div{
            margin: 10px 0;
        }
        .div3{
            border-left: none;
        }
        .div3::before{
            content: "";
            position: absolute;
            width: 130px;
            height: 2px;
            transform: translateY(-20px);
            background-color: #5883af;
            margin: 0px 0;
        }
    }
    @media (max-width:390px){
        .div2 a{
            font-size: 0.8rem;
            padding: 5px 5px;
        }
    }
</style>