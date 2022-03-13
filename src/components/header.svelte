<script>
    
    function menuopen(){
        document.getElementById("nav").classList.toggle("navopen");
    }
    window.addEventListener("resize", function(event) {
        if(document.body.clientWidth>830){
            document.getElementById("nav").classList.add("navopen");
        }
    });
    
</script>
<div class="main ">
    <div class="exclass">
        <div class="left ">
            <img src="./assets/img/logo.png" alt="" height="70px"/>
        </div>
        <div class="right ma">
            <div class="large">
                <a href="#" class="active">home</a>
                <a href="#">Protection&nbsp;and&nbsp;Features</a>
                <a href="#">Pricing</a>
                <a href="#">About</a>
                <a href="#">Blog</a>
                <a href="#">Contact&nbsp;Us</a>

            </div>
            <div id="navbtn" on:click="{menuopen}"><i class="fas fa-bars"></i></div>
        </div>
    </div>
    <div class="small navopen" id="nav">
        <a href="#">Home</a>
        <a href="#">Protection&nbsp;and&nbsp;Features</a>
        <a href="#">Pricing</a>
        <a href="#">About</a>
        <a href="#">Blog</a>
        <a href="#">Contact&nbsp;Us</a>
    </div>
</div>
<style>
    .small,#navbtn{
        display: none;
    }
    .ma{
        margin-left: auto;
        margin-right: auto; 
    }
    .left{
        margin: 0 0 0 5vw;
    }
    .main{
        overflow: hidden;
        height: 74px;
    }
    .exclass{
        display: grid;
        z-index: 100;
        grid-template-columns: 1fr 2fr;
        background: #333;
    }
    .right .large a{
        align-content: center;
        transition: all 0.2s;
        padding:0 5px;
        height: 30px;
        margin: 15px 0;
        padding: 10px;
        display: inline-grid;
        text-decoration: none;
        color: #bbb;
    }
    .right .large a:hover{
        background: rgb(71, 71, 71);
    }
    .active{
        color: red !important;
    }
    @media (max-width:830px){
        .small,#navbtn{
            display: grid;
            color: white;
        }
        .right{
            margin: 0;
        }
        #navbtn{
            padding: 20px;
            width: 16px;
            margin: 10px 0 8px auto;
            border-radius: 50%;
        }
        #navbtn:hover{
            background: #424242;

        }
        .large{
            display: none;
        }
        .small{
            background: #333;
            position: absolute;
            height: 240px;
            overflow: hidden;
            transition: all 0.5s;
            /* margin-top: 80px; */
        }
        .small>a{
            text-decoration: none;
            transition: all 0.5s;
            display: block;
            padding: 5px 0 5px 5vw ;
            color: #bbb;
            width: 95vw;
            height: 30px;
            align-content: center;
        }
        .small a:hover{
            background: #424242;
            letter-spacing: 1px;
        }
        .navopen{
            height: 0px;
        }
    }
</style>