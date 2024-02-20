# Resumo do Projeto de Organização de Computadores I

O projeto visou a implementação das instruções ANDI, MUL, DIV e BEQ em um ambiente Risc-V pré-configurado, exigindo modificações nos arquivos de tradução de instruções, na unidade de controle e na ALU. A implementação começou com a análise do pipeline e do esquema, seguida de ajustes na unidade de controle para incorporar tratamento de OPCode e na ALU para realizar as operações corretas.

Para a instrução ANDI, foram feitas alterações na unidade de controle e na ALU para realizar a operação lógica AND com o imediato. As instruções MUL e DIV foram implementadas de forma paralela, adicionando códigos de OPCode, Funct3 e Funct7, e ajustes na ALU para executar as operações de multiplicação e divisão.

A instrução BEQ exigiu tratamento do OPCode, captura do imediato e operação de subtração na ALU. A análise detalhada dos elementos nos pipelines, como branch_eq, baddr_s2_s3 e outros, foi essencial para o sucesso da implementação.

Testes foram realizados para verificar o funcionamento correto das instruções, abordando casos como ANDI com registradores pares e ímpares, MUL com valores específicos, DIV com valores distintos e BEQ com valores iguais e diferentes.

A conclusão destaca o aprendizado significativo, desde a compreensão do pipeline até a integração eficaz das novas instruções. O projeto ressaltou a importância da linguagem Verilog e a necessidade de uma estruturação cuidadosa do pipeline para uma implementação bem-sucedida.
