# ME17.5.24 — Labels para VCDS

Este repositório fornece labels para o scanner VCDS compatíveis com a ECU/Módulo de injeção ME17.5.24 encontrada em modelos como Novo Gol, Fox, Voyage e Saveiro (a partir de 2013).

Objetivo: disponibilizar uma label funcional que facilite a leitura de blocos de dados para realizar diagnósticos em veículos equipados com a ECU ME17.5.24.

**Informações principais**

- **ECU:** ME17.5.24        03 1405  
- **HW:** 030 907 309 A
- **Part No SW:** 030 906 020 E 
- **Veículo Testado:** VW Novo Gol 2014 1.0 TEC 4 Cilindros CPBA com ECU Bosch ME17.5.24.
- **Versão do VCDS:** VCDS 24.5.0 (pode ser compatível com outras versões)

## Aviso sobre as labels

Algumas labels incluídas neste repositório foram obtidas a partir de outros modelos/ECUs a procura de labels que funcionem. No entanto, essas labels não foram criadas especificamente para esta ECU. Proceda com extrema cautela principalmente se for modificar algo em adaptations/basic settings por sua conta e risco.

## Instalação

1. Baixe o repositório como um .zip

Para baixar como ZIP: abra a página deste projeto no GitHub, clique em "Code" → "Download ZIP", salve e extraia o arquivo;

2. Copie a label de referência

    - Abra a pasta `Labels` do repositório.
    Copie a label de referência (por exemplo `03C-906-024-BXW.lbl`) para a pasta de labels do VCDS, normalmente `C:\Ross-Tech\VCDS\Labels`. Se já existir uma label com o mesmo nome, não é necessário sobrescrever salvo se você quiser atualizar a label.

3. Copie a label de redirecionamento (User)

	- Abra a pasta `Labels/User` do repositório.
	- Copie os arquivos para `C:\Ross-Tech\VCDS\Labels\User`
	- A label de redirecionamento é necessário para que o VCDS associe a ECU às label na pasta `\Labels`.
    - Alternativamente, você pode copiar a label de referência e renomea-la para o part number da ECU para que o VCDS detecte ela, que no caso é `030-906-020-E.lbl`.
 

## Solução de problemas

- VCDS não exibe a label: verifique se os arquivos foram colocados nas pastas corretas e reinicie o VCDS. 
- Faça um Scan e verifique se o part number da sua ecu é o 030-906-020-E, se não for, renomeie a label em Labels/User para o part number da sua ECU e teste para ver se a label funciona.

## Contribuição

Contribuições são bem-vindas.
## Contato

Se tiver dúvidas, reporte uma issue ou entre em contato no repositório.