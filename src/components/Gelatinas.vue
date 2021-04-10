<template>
    <div>
        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootswatch/4.5.2/journal/bootstrap.min.css" integrity="sha384-QDSPDoVOoSWz2ypaRUidLmLYl4RyoBWI44iA5agn6jHegBxZkNqgm2eHb6yZ5bYs" crossorigin="anonymous">
        
        
        <div class="container mb-4">
            
            <div class="row justify-content-between">
                <div class="col-4">
                    <!-- <img class="ml-2" src="https://bn1303files.storage.live.com/y4mGVvgLUjB4_xbJbfy5K8MbShtMpBV5aRXTzQ61OOtRKFfLRewp14RacWpiVZxDGyt_KMRI5b-j69i8Fgk8E8iUpKYfSaw41H3PWTJO64lGSytDoLImzo8D7NK3keeRVCP2vi6uteJ1762Grk6p59njcV2qZqgCf7aS0o6v2LrfBLEI147bj1UGF9bQ34TnZQ9?width=64&height=64&cropmode=none" width="30" height="30" alt=""> -->
                    <a class="navbar-brand ml-2 font-letras" href="#">Antojitos Karina</a>
                    
                </div>
                <div class="col-4">

                    <a  href="https://www.facebook.com/Antojitos-Karina-105819398281943">
                        <img class="navbar-brand" src="https://bn1303files.storage.live.com/y4mDWEfv1BTvKKB1lFwEJe-miq1mxhnBp_KUiVGpnsrfxZ_okZ4OZkxx8uGYTbI9VcYCoHhy5lbJZvOMsOhk7vI4mhi0pWWruOX5-oLEbcq-T5JF11bfjNAfcALysHthZlpSzg3zSejcPn2sBpjrE0yeI3F1R1g7syHXEX_NFq2LbN88k5i60qkW8qgobzfJ7Eu?width=32&height=32&cropmode=none" alt="">
                        <img class="navbar-brand" src="https://bn1303files.storage.live.com/y4m4QTj_H3jdtYSKbKKp7flrU1tN0FsOet-ogLIRP2Wq1PUjaLe0XndXrXmFzyvSBl-Ia1naKiVyv2ZNE_Uc9PbdTzob8YcNCrY18iztDO6l_gNKVM9sDjhQvcv37LBqjKWML1uRnOrF_K5MmuoUOFpxrq1G_Q9WZhJvkjSOZabahVzMm9pCJ89jwO-cGojf0oX?width=32&height=32&cropmode=none" alt="">
                    </a>
                </div>
            </div>

            <div class="row justify-content-center">
                <ul class="nav nav-pills mt-4">
                    <li class="nav-item">
                        <a class="nav-link active" href="#">GELATINAS</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link disabled" href="#">POSTRES</a>
                    </li>
                </ul>
            </div>
            <div class="row">
                <div class="col col-lg-4 col-md-6 col-sm-12"  v-for="gelatina in gelatinas" :key="gelatina.nombre">
                    <div class="card border-primary mt-3 ">
                        <!-- <div class="card-header bg-primary font-letras"></div> -->
                        <div class="card-body">
                            <h4 class="card-title font-letras">{{gelatina.nombre}}</h4>
                            <img class="img-thumbnail" :src="gelatina.img" alt="" width="304" height="236">
                            <p class="bg-primary form-control"> <span class="ppp"> S/. {{gelatina.precio}}</span></p>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Whatsapp -->
            <a href="https://api.whatsapp.com/send?phone=51910660658&text=%F0%9F%98%81%20%22Hola%2C%20quiero%20saber%20mas%20informaci%C3%B2n%20sobre%20las%20gelatinas%22"
                class="btn-whatsapp" target="_blank">
                <img class="icon-whatsapp" src="https://bn1303files.storage.live.com/y4mUcfTYbgX6x3CwOTAZ992fNOoJbhwFVm5SVHn7ooQFw9qiJ7ePZFsWrTiXkoTcpovuCEDYd8gj9DG2XO7KHIsx3C8aAZ_pPJWvE-8y4NRdzv5u89XmJ3IDGKzYvoTtPlNEylsI_QY_en7uNr_WslWUZtYTSS9siMpM4weBCmnVPE5E2oil1GaAjofk5ixPUqr?width=24&height=24&cropmode=none" alt="">
            </a>
            
            
        </div>
    </div>
</template>

<script>

export default {
    data(){
        return{
            msg:'Hola Xd',
            gelatinas:[
                {
                    nombre:'Arco Iris', 
                    img:'https://bn1303files.storage.live.com/y4mf8Ww2ZIbLqw4lpUGvpv9dXoR_XO68S5CcO2pU7Sx0HB80UspnUlrvvqe_szStcBzDnyzsnMMYkHAaca4USBlGStluSzmBFI1y4k60aRuDExTp1z2Yc6f_vDdHzzQmKZdyEHPd3C7B3r5gMtLIpW4lXVv491ALc1hmmvc_eg839M522EWJWYF7hsN7wb7CYBd?width=289&height=354&cropmode=none',
                    descripcion:'descripcion de Gelatina 1',
                    precio: 2.00
                },
                {
                    nombre:'Payaso', 
                    img:'https://bn1303files.storage.live.com/y4min7LxK3vcAFtvMzTgAE1w0iJSqymeCucnC9DsW0naerZcm_B0v7r83nAAJtt5lIS9IZFoqui5qDUG7QbuMuxQQ2I7als5dMa4wt92SNmn1c9_T0JkxsLBqawYznyYDwUfuI7rdsPB7yeYAc8V_NIEBBguZnWXF3ieDRfdrACN5ThjBZDLjFMCwaPUcQ7Dz89?width=319&height=391&cropmode=none',
                    descripcion:'descripcion de Gelatina 1',
                    precio: 2
                },
                {
                    nombre:'Gelatina con Flan', 
                    img:'https://bn1303files.storage.live.com/y4mQTcNR2PUkh8iB-jFp-wu7hzjOftTedaCp8v-RmBj3Y7CRUjKU6ki5SIN0DhhxuhF79e0EewhextaWupcDYSKKck9hzhWb-xOLDOfyvhHyGELACFhEEysJpf9Q_6A7s2Q1YOwWZ8QUacEbH3PiXI-OWkiyJmDTRdXrYoVvN7l9EC0yq-7hzUqfAogwZobyh6k?width=327&height=400&cropmode=none',
                    descripcion:'descripcion de Gelatina 1',
                    precio: 1
                },
                {
                    nombre:'GelaFlan', 
                    img:'https://bn1303files.storage.live.com/y4mjhX0g4pgsDc0VlWIuHVljfjWnfARsDubbM720h28Vsi0WinGCikyvqxV0HkyWZGFTNXfBlp934eFvKVVfw9m13cxPRc1RwOCwESMgyoX3s2PVYQbF0VSeKacLV6VbH_rmxVropuqlf7ForSLw004F14QA0ZClMhKQxiMwlZe4jeDlh1nXgXDKmcqFmtHdJiN?width=341&height=419&cropmode=none',
                    descripcion:'descripcion de Gelatina 1',
                    precio: 1.5
                },
                {
                    nombre:'Carlota', 
                    img:'https://bn1303files.storage.live.com/y4mjmmPIrybKpktS8c-C7iHFFPAEdZ4lz4J5GxFGGIB6v3xvARNf5N-A1vhpbxRdphLDDDZxukuqxa9fVCOD4jq0hnWBe8_LDTuTkZF4jBCMh5FdR9uj74ox1PcDm28aH2G3owqVZM01FYX4PcvzMlUFVmvf4YqbpBYHxHW1Hf-wY8CRBox1LwKLjenLf-V0QBY?width=278&height=342&cropmode=none',
                    descripcion:'descripcion de Gelatina 1',
                    precio: 1.5
                },
                {
                    nombre:'Chocoflan', 
                    img:'https://bn1303files.storage.live.com/y4mwDtO10Ne3SCIVvW15VTX4w4j4sk6qwL1XdghEOds2Hq-sTgbv2e-Nyu_hD6Nm40APjBM4N_bFk-0LK-awqoOlKld2ttI8nziTPQMo8j-_nKCeH1lJKoKNbwaDL1ncTAWaQAwwUUEpM203eCovl94mgZ3LGwhztSOJWoAbWaHwLBQNffga93zucrom0XPyAEl?width=319&height=391&cropmode=none',
                    descripcion:'descripcion de Gelatina 1',
                    precio: 1.5
                },
                {
                    nombre:'Chocoflan con Crema', 
                    img:'https://bn1303files.storage.live.com/y4mARXQ7CnrWWPb7b8VZcZpWuTRn3urwOpHlUvTjxXLWYoxI-V0is0QYAXKAETO15AuTB9k4xTQpadYgHe33f-EMbwaEh0eNtLVCLKSXpmN6atUe8wyTo0MErM3X5HeiK4eFGKBUjp2lDaj0tgwoDmkUmSvdk-4tEbPxbNP4A1L3csO3ZZXoyYrJluiSm5YGoR7?width=319&height=391&cropmode=none',
                    descripcion:'descripcion de Gelatina 1',
                    precio: 2.0
                },
                {
                    nombre:'Gelatorta con crema 1', 
                    img:'https://bn1303files.storage.live.com/y4m0nP8blAczQ8zbmOZT2cufKzGFgjNrpbh6ajbaGkkN4rYFt7qbLbRihJU_2JkIdHkmybpRaq9FiFx5m88p9pmY26zdDPXAVCsC_FmqiIW1Qe4diNfaoeSl4hde182piD52XrRjUK3Rix-KhS-PJFJCw5sLhZpEYIHJMSgPN91gKcgoM_gDFmz_djA9kxcwKb4?width=306&height=406&cropmode=none',
                    descripcion:'descripcion de Gelatina 1',
                    precio: 2.0
                },
                {
                    nombre:'Gelatorta con crema 2', 
                    img:'https://bn1303files.storage.live.com/y4mXV13PXFSm7fsIYt1w6fvSp3xnYp_m14VFpYyMp1k0mX24I7DLY0gk-GF32fzh9cUQ6kSjxzjMOr_Q71lo8o-wdDu2P38vlawbGVtP3qvprY1URWoAdMR_9ZqneqjV6VpyivL6W2DAuMVi7i6EsVRGznw8ZDC-aG2lhSNo_Dxu6LV23akGCvNvfMhbcIKJWrk?width=306&height=406&cropmode=none',
                    descripcion:'descripcion de Gelatina 1',
                    precio: 2.0
                },
                {
                    nombre:'Fresa, Piña y Naranja', 
                    img:'https://bn1303files.storage.live.com/y4mGdsoC-4SZ1RXWqQdBjKPAVusTcyimAAlisSkBoLsyGogS3lJ8M1LoywIbOLTfB2huZl1_V0MmpTrJsHlKIaBV3HA1VQEkXsZVeCZ92ruqyUlfjJEGNkYjnTocI5k7Jeolw8G0tCUWNXaxw54ukBNpiYLusqQE7JdzV6yduLJoU6-YGFN3MLx0xhayYMkS27u?width=345&height=423&cropmode=none',
                    descripcion:'descripcion de Gelatina 1',
                    precio: 1
                }
            ]
        }
    },
    methods:{}
}
</script>

<style>

.grid{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1rem;
    justify-items: stretch;
}

@import url('https://fonts.googleapis.com/css2?family=Handlee&display=swap');

.font-letras{
    font-family: 'Handlee', cursive;
    font-size: 1.9rem;
    color: #e2372b;

}

.ppp{
    color:beige;
    font-size: 1.3rem;
    font-weight: bold;
}

/* boton flotante */

.btn-whatsapp{
    position: fixed;
    width: 50px;
    height: 50px;
    line-height: 50px;
    bottom: 40px;
    right: 40px;
    background: #0df053;
    color: gainsboro;
    border-radius: 50px ;
    text-align: center;
    font-size: 2px;
    box-shadow: 0px 1px 10px rgba(0, 0, 0, 0.3);
}

.btn-whatsapp:hover{
    text-decoration: none;
    color: #0df053;
    background: #fff;
}

/* e2372b */
</style>