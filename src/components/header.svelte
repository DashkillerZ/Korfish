<script>  
    import {createEventDispatcher} from 'svelte';
    let dispach = createEventDispatcher();

    function handleClick(i){
        dispach('handle', i);
        // console.log(i);
    }

</script>
<div class="main ">
    <div class="left" on:click={()=>{handleClick(0)}}>
        <img src="./assets/img/logo.svg" alt="" height="55px"/>
    </div>
    <details>
        <summary>
            <span>Explore Features</span>
            <div>
                <div></div>
                <div></div>
                <div></div>
            </div>
        </summary>
        <div class="menu">
            <a href="#" on:click={()=>{handleClick(1)}}>Bad Bots</a>
            <a href="#" on:click={()=>{handleClick(2)}}>Bad Words</a>
            <a href="#" on:click={()=>{handleClick(3)}}>Proxy Protection</a>
            <a href="#" on:click={()=>{handleClick(4)}}>Spam Protection</a>
            <a href="#" on:click={()=>{handleClick(5)}}>SQLi Protection</a>
        </div>
    </details>
</div>
<style>
    .main{
        height: 80px;
        display: flex;
        background: #333;
        justify-content: space-between;
    }
    .left{
        display: flex;
        align-items: center;
        padding-left: 6vw;
    }
    .menu{
        display: grid;
        position: absolute;
        background:#333;
        width: 180px;
    }
    .menu a{
        padding: 13px 0 0px 20px;
        text-decoration: none;
        color: white;
        font-size: 1.2rem;
        transition: all 200ms;
        height: 40px;
        align-items: center;
    }
    .menu a:hover{
        text-decoration: none;
        color: red;
        font-size: 1.2rem;
        background: #444;
    }
    details{
        display: flex;
        align-items: center;

    }
    summary{
        align-self: center;
        color: white;
        font-size: 1.3rem;
        list-style: "";
        height: 50px;
        margin: 27px 6vw 0 0;
        padding:  0 10px ;
        border-bottom: 3px solid red;
        cursor: pointer;
        user-select: none;
    }
    summary div{
        display: none;
        width: 30px;
    }
    summary>div div{
        width: 28px;
        height: 3px;
        border-radius: 2px;
        margin: 6px auto;
        background: white;

    }
    @media (max-width:580px){
        .menu{
            width: 100vw;
            position: absolute;
            left: 0;
        }
        summary span{
            display: none;
        }
        summary div{
            display: block;
        }
    }
  
</style>