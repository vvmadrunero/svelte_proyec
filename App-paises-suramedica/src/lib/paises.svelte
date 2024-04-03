<script>
    export let pais;
    let p;
    const paises={
    "Colombia ":["Colombia","Bogota","51,52 millones","Pesos Colombianos"],
    "Venezuela":["Venezuela","Caravas","28,2 millones","Bolivar"],
    "Ecuador":["Ecuador","Quito","17,8 millones","Dolar estaunidense"],
    }
    p=paises[pais];
</script>
<div class="main" >
    <div class="col1">
        <img src="./src/assets/{p[5]}" alt="Bandera_Colombia"width="300" height="200">
    </div>
<div class="col2">
    <div class="linea"><strong>pais:</strong>{p[0]}</div>
    <div class="linea"><strong>capital:</strong>{p[1]}</div>
    <div class="linea"><strong>poblacion:</strong>{p[2]}</div>
    <div class="linea"><strong>moneda:</strong>{p[3]}</div>


</div>
</div>


<style>
    .main {
        display: grid;
        grid-template-columns: repeat(4,1fr);
        grid-gap:5px;
        grid-auto-rows: minmax(100px, auto);
        border-radius: 10px;
        border-style: solid;
        border-color: rebeccapurple(239,190,20);
        border-width: 2px;
        margin: left;
        width: 600px;
        box-shadow: 5px 5px 5px black;
        margin-right: 5px;
        margin-bottom: 10px;

    }
    .col1 {
        grid-column: 1;
        grid-row: 1;
        margin: 5px;
        padding: 5px;
    }
    .col2 {
        grid-column: 2;
        grid-row: 2;
        margin: 5px;
        padding: 5px;
        border-color: black;
        width:max-content;

    }
    strong {
        color: magenta;
        font-weight: bolder;

    }
    .linea{
        font-size: 20px;
        margin-bottom: 18px;
    }

</style>

