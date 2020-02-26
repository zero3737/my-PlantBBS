<template>
   <div class="index">
       <Header></Header>
       <Nav></Nav>
       <Neirong1></Neirong1>
       <Lunbotu></Lunbotu>
       <Neirong2></Neirong2>
       <Tuijian></Tuijian>
       <Banquan></Banquan>
   </div>
</template>

<script>
import Header from "./Header"
import Nav from "./Nav"
import Neirong1 from "./Neirong-1"
import Banquan from "./Banquan"
import Lunbotu from "./Lunbotu"
import Neirong2 from "./Neirong-2"
import Tuijian from "./Tuijian"

export default {

    components: {

        Header,
        Nav,
        Neirong1,
        Banquan,
        Lunbotu,
        Neirong2,
        Tuijian

    }
    
}
</script>