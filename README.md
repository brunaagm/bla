index: 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora Bruna</title>
</head>
<body>
    <h1>Menu de operações </h1>
    <select id="operações" name="operações" required>
        <option value="select"> Selecione </option>
        <option value="add"> Adição </option>
        <option value="sub"> Subtração </option>
        <option value="multi"> Multiplicação </option>
        <option value="divi"> Divisão </option>
    </select> 
    
    <input type="number" id="num1" placeholder="Digite o número 1">
    <input type="number" id="num2" placeholder="Digite o número 2">
    <button onclick="Calcular()"> Calcular</button>
    
    
    <h2 id="resultado"></h2>
    
    
    <script src="script.js"> </script>



</body>
</html>


script:
function calculadora(num1, num2, operador) {
    let resultado

    switch (calculo) {
        case 'add':
            resultado = num1 + num2;
            break;
        case 'sub':
            resultado = num1 - num2;
            break;
        case 'multi':
            resultado = num1 * num2;
            break;
        case 'div':
            if (num2 !== 0) {
                resultado = num1 / num2;
            } else {
                return 'Erro: Divisão por zero';
            }
            break;
        default:
            return 'Calculo inválido';
        
        case 'sqrt':
            if (num1 >= 0) {
                resultado = Math.sqrt(num1);
            } else {
                return 'Erro: Não é possível calcular a raiz quadrada de um número negativo';
            }
            break;
        }
    }
    document.getElementById("resultado").textContentt = "resultado: " + resultado


    
const num1 = parseFloat(document.getElementById("num1").value);
const num2 =  parseFloat(document.getElementById("num2").value);


document.getElementById("resultado").textContentt = "resultado: " + resultado


css: 




