<template>
    <div id="maps">
    <router-link to="/"><b-icon icon="x" class="back" style="width: 30px; height: 30px;  margin-right: 0.4em; color: black; float: right;"></b-icon></router-link>          
    
    <h2>* locations</h2>  
        <b-card no-body>
        <b-tabs pills card vertical nav-wrapper-class="w-50">
            <b-tab title="AJ Katzenmaier" active><b-card-text>24 W. Walton St., Chicago, IL 60610</b-card-text></b-tab>
            <b-tab title="Greenbay"><b-card-text>1734 N. Orleans St., Chicago, IL 60610</b-card-text></b-tab>
            <b-tab title="Howard A Y"><b-card-text>2245 N. Orleans St., Chicago, IL 60610</b-card-text></b-tab>
            <b-tab title="Marjorie P H"><b-card-text>2625 N. Orchard St., Chicago, IL 60610</b-card-text></b-tab>
            <b-tab title="North"><b-card-text>1409 N. Ogden Ave St. Chicago, IL 60610</b-card-text></b-tab>
            <b-tab title="South"><b-card-text>2101 N. Fremont St., Chicago, IL 60610<br></b-card-text></b-tab>
        </b-tabs>
        </b-card>
    </div>
</template>

<script>

</script>

<style>

.titulazo{
    font-family: helvetica;
    font-weight: bold;
    text-align: center;
    margin: 5vh;
}

.card{
    border: none;
}
.card-text{
    margin-top: 50%;
}

.nav-pills .nav-link.active{
    background-color: #b0c8f3;
    color: black;
    width: 100%;
    border: none;
}

.nav-link{
    color: #b1b6bd;
}
</style>