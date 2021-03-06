# Novidade do .NET5 com C#9

Problemas recorrentes, resolvidos muitas vezes, geralmente têm soluções implementadas de maneira similar. Em implementações de DTOs, somente para leitura, por exemplo, é comum:

- definir construtores onde cada parâmetro corresponde a uma das propriedades do tipo;
- implementar versões customizadas da função de igualdade;
- definir métodos auxiliares para criação de novas instâncias a partir de outras existentes.

O código, mesmo que escrito no “piloto automático” por programadores mais experientes, abre possibilidade para erros de codificação e lógica, demandando, para evitar prejuízos, a escrita de mais testes de unidade.

A evolução da C# tem trazido para a linguagem a solução de problemas recorrentes tornando as implementações menos imperativas e mais declarativas.

Na C# 9, por exemplo, teremos:

- init-only properties que tornaram desnecessários construtores apenas para a inicialização dos campos;
- O modificador data que, entre outras coisas, fornecerá implementações especializadas de Equals e GetHashcode;
- with-expressions que permitirá criação de novas instâncias a partir de outras existentes;
- new-expressions que inferem o tipo de um objeto a partir do tipo declarado para a variável.
Tudo isso deixando o código muito mais breve.

Aliás, o método Main tornou-se opcional. A partir da C# 9, há suporte direto para o que o time da Microsoft chama top level programs. Nesses cenários, o parâmetro args continua disponível implicitamente.

Finalmente, há ainda uma novidade que permite tornar a construção de DTOs ainda mais econômica. São os positional records.

Referência
https://docs.microsoft.com/pt-br/dotnet/csharp/whats-new/csharp-9
