<script>
    export let numero; //
    let resultado; 
    $: if (numero===0)
        resultado=" Neutro ";
    else
        if (numero%2===0)
        resultado=" Par";
    else
        resultado=" Impar ";
    
    </script>
    <!--Las variables se deben de llamar entre llaves-->
    <p> El numero {numero} Es {resultado} </p>
    <style>
        p{
            color: rgb(242, 10, 10);
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            font-size: 27px;
        }
    </style>
    
    
    