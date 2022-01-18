# Um pouco sobre as PSRs (PHP Standards Recomendations)

# PSR 0

## PSR 1
PSR sobre recomendações básicas de codificação.

* As as tags PHP devem ser ```<?php ?>```  ou  de forma abreviada ```<?= ?>```, nenhuma outra forma deve ser utilizada! 
* A codificação deve ser apenas e,m UTF-8

* Não usar código que possam causar efeitos colaterais, como:
```
<?php
// efeito colateral: muda as configuraões de inicialização
init_set('error_reporting', E_ALLL);

// efeito: carrega um arquivo
include "file.php";

// efeito: gera saida
echo "</html>";

// efeito: declara uma função

function foo()
{
    // corpo da função
}
```