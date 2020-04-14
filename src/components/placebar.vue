<template>
    <div class="info">
        <h2 class="title has-text-white">Dina närmsta barer:</h2>

    <ul class="places columns">
        <li class="place column">
            <p class="name is-size-5">Paddington's</p> <p class="adress is-size-7">Sankt Pauligatan 1, 416 60 Göteborg</p> <p class="openinghrs">Closed. Opens 16:00</p> <p class="price has-text-primary">$</p> <a href="https://www.google.com/maps/dir/Lernia+G%C3%B6teborg+-+Lediga+jobb,+bemanning+%26+utbildning/Paddington's,+Sankt+Pauligatan,+Gothenburg/@57.7105776,11.9917135,17.19z/data=!4m13!4m12!1m5!1m1!1s0x464ff3802866d1fd:0xf16567aaacb71c6b!2m2!1d11.9943241!2d57.709833!1m5!1m1!1s0x464ff47f297d08ab:0xb54eb8d3df48025d!2m2!1d12.0042479!2d57.7137576" class="button has-background-info">Hitta hit!</a>
        </li>
        <li class="place columns">
            <p class="name is-size-5">Ostindiska Ölkompaniet</p> <p class="adress is-size-7">Danska vägen 110, 416 59 Göteborg</p> <p class="openinghrs">Closed. Opens 15:00</p> <p class="price has-text-primary">$$$</p> <a href="https://www.google.com/maps/dir/Lernia+G%C3%B6teborg+-+Lediga+jobb,+bemanning+%26+utbildning/Ostindiska+%C3%96lkompaniet,+Danska+v%C3%A4gen,+Gothenburg/@57.7105776,11.9917135,17.19z/data=!3m1!4b1!4m13!4m12!1m5!1m1!1s0x464ff3802866d1fd:0xf16567aaacb71c6b!2m2!1d11.9943241!2d57.709833!1m5!1m1!1s0x464ff47ecfa687e3:0x356ce36c3a8700c7!2m2!1d12.0044408!2d57.7149763" class="button has-background-info	">Hitta hit!</a>
        </li>
        <li class="place column">
            <p class="name is-size-5">Ölstugan Tullen</p> <p class="adress is-size-7">Friggagatan 27, 416 64 Göteborg</p> <p class="openinghrs">Closed. Opens 15:00</p> <p class="price has-text-primary">$</p> <a href="https://www.google.com/maps/dir/Lernia+G%C3%B6teborg+-+Lediga+jobb,+bemanning+%26+utbildning/%C3%96lstugan+Tullen+%F0%9F%8D%BA,+Friggagatan,+Gothenburg/@57.7105776,11.9917135,17.19z/data=!3m1!4b1!4m13!4m12!1m5!1m1!1s0x464ff3802866d1fd:0xf16567aaacb71c6b!2m2!1d11.9943241!2d57.709833!1m5!1m1!1s0x464ff48010000001:0x8c5929ddaf2732ae!2m2!1d11.9910928!2d57.7124804" class="button has-background-info	">Hitta hit!</a>
        </li>
        <li class="place column">
            <p class="name is-size-5">Franke's</p> <p class="adress is-size-7">Alströmergatan 3B, 411 01 Göteborg</p> <p class="openinghrs">Closed. Opens 15:00</p> <p class="price has-text-primary">$$</p> <a href="https://www.google.com/maps/dir/Lernia+G%C3%B6teborg+-+Lediga+jobb,+bemanning+%26+utbildning/Franke's,+Alstr%C3%B6mergatan,+Gothenburg/@57.7105776,11.9917135,17.19z/data=!3m1!4b1!4m13!4m12!1m5!1m1!1s0x464ff3802866d1fd:0xf16567aaacb71c6b!2m2!1d11.9943241!2d57.709833!1m5!1m1!1s0x464ff37e46b0b9d5:0xd400f47cc8cdd14b!2m2!1d11.9882979!2d57.710916" class="button has-background-info	">Hitta hit!</a>
        </li>
        <li class="place columns">
            <p class="name is-size-5">Glenn Sportsbar</p> <p class="adress is-size-7">Friggagatan 9, 411 01 Göteborg</p> <p class="openinghrs">Closed. Opens 16:00</p> <p class="price has-text-primary">$$</p> <a href="https://www.google.com/maps/dir/Lernia+G%C3%B6teborg+-+Lediga+jobb,+bemanning+%26+utbildning/Glenn+Sportsbar,+Friggagatan+9,+411+01+G%C3%B6teborg/@57.7105908,11.9934547,17.71z/data=!4m13!4m12!1m5!1m1!1s0x464ff3802866d1fd:0xf16567aaacb71c6b!2m2!1d11.9943241!2d57.709833!1m5!1m1!1s0x464ff37e64dadbc9:0x1a93f95de6f23a2f!2m2!1d11.9868697!2d57.7104199" class="button has-background-info">Hitta hit!</a>
        </li>
    </ul>

    </div>


</template>

<script>
export default{
    name: 'places',
}
</script>

<style scoped lang="scss">

.info{
    background: linear-gradient(rgb(255, 123, 0), rgb(255, 196, 108));

    .title{
        text-align: left;
        padding: 15px;
        margin-left: 15px;
    }

    ul{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        li{
            padding: 15px;
            width: 95%;
            margin: 15px 0;
            height: auto;
            text-align: left;
            background-color: whitesmoke;
            box-shadow: 7px 5px 5px rgba(107, 107, 107, 0.534);
            display: flex;
            flex-direction: row;
            justify-content: center;
            align-items: center;

            .name{
                color: #F1A624;
                width: calc(100%/5);
            }
            .adress{width: calc(100%/5); margin: 15px 0;}
            .openinghrs{width: calc(100%/5);}
            .price{width: calc(100%/5);}
            .button{
                margin: 20px 0;
                color: white;
                width: 175px;
                width: calc(100%/5);
                cursor: pointer;
                
            }
        }
    }
}
@media screen and (max-width: 500px) {
.info{
    background: linear-gradient(rgb(255, 123, 0), rgb(255, 196, 108));

    .title{
        text-align: left;
        padding: 15px;
        margin-left: 0;   
    }

    ul{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        li{
            padding: 15px;
            width: 95%;
            margin: 15px 0;
            height: auto;
            text-align: left;
            background-color: whitesmoke;
            box-shadow: 7px 5px 5px rgba(107, 107, 107, 0.534);
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;

            .name{
                color: #F1A624;
                width: auto;
            }
            .adress{width: auto;}
            .openinghrs{width: auto;}
            .price{width: auto; margin: 5px 0;}
            .button{
                margin: 20px 0;
                width: 75%;
            }
        }
    }
}
}
    
</style>
