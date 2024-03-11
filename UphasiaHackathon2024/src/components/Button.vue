<template>
        <div style="display: block;">
            <div>
                <a href="https://docs.google.com/forms/d/e/1FAIpQLSc_DuP2e0Gaj5EJ6yY3dOUSgCNvH17Oiy-xr5azo9YtopaETg/viewform?usp=sf_link">
                <button id="register" > ลงทะเบียน</button>
            </a>
            </div>
            <div>
                <a href="mailto:contact@uphasia.co">

                    <button id="contact">ติดต่อเรา</button>
                </a>
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
        min-width: 200px;
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
        min-width: 200px;
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