<template>
        <div style="display: block;">
            <div>
                <button id="register">ลงทะเบียน</button>

            </div>
            <div>

                <button id="contact">ติดต่อเรา</button>
            </div>

        </div>

</template>

<style scoped>
    #register{
        margin: 5px;
        cursor: pointer;
        font-family: "Kanit", sans-serif;
        font-style: normal;  
        background-color: #17AA7C;
        color: white;
        font-size: 3vh;
        width: 25vmin;
        padding: 10px;
        border-radius: 10px;
        border: 3px solid rgba(0, 0, 0, 0.332);
    }
    #contact{
        cursor: pointer;
        font-family: "Kanit", sans-serif;
        font-style: normal;  
        background-color: white;
        color: #121212a0;
        font-size: 3vh;
        width: 25vmin;
        padding: 10px;
        border-radius: 10px;
        border: 3px solid rgba(0, 0, 0, 0.332);
    }
    #register:hover{
        cursor: pointer;
        transition: all .2s;
        background-color: #10674b;

    }
    #contact:hover{
        cursor: pointer;
        transition: all .2s;
        background-color: rgb(229, 229, 229)    }
</style>