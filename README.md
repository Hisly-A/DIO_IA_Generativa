# IA Generativa
Explorando os Recursos de IA Generativa com Copilot e OpenAI.

## Copilot
### O que é?
>O Copilot é uma ferramenta de produtividade alimentada por IA que usa LLMs (grandes modelos de idioma), um tipo de algoritmo de IA (inteligência artificial) que usa técnicas de aprendizado profundo e vastos conjuntos de dados para entender, resumir, prever e gerar conteúdo. Esses LLMs incluem modelos pré-treinados, como Transformadores Pré-Treinados Generativos (GPT), como GPT-4, projetados para se destacar nessas tarefas. Essa integração fornece assistência inteligente em tempo real, permitindo que os usuários aprimorem sua criatividade, produtividade e habilidades.

<sub>Fonte: <https://learn.microsoft.com/pt-br/microsoft-365-copilot/microsoft-365-copilot-overview></sub>

### Como utilizar?
Podemos fazer solicitações ao Copilot usando linguagem natural, como por exemplo, na imagem abaixo foi silicitada a geração de um código de calculadora em Java:

![solicitado1](https://github.com/Hisly-A/DIO_IA_Generativa/assets/inputs/inputcopilot%2001.PNG)

Como resultado, o Copilot retornou o seguinte código:

![retorno1](https://github.com/Hisly-A/DIO_IA_Generativa/assets/outputs/outputcopilot%2001.PNG)

```
import java.util.Scanner;

public class Calculadora {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        System.out.println("Digite o primeiro número:");
        double num1 = scanner.nextDouble();

        System.out.println("Digite o segundo número:");
        double num2 = scanner.nextDouble();

        System.out.println("Digite a operação ( + , - , * , / ):");
        char operacao = scanner.next().charAt(0);

        scanner.close();
        
        double resultado;

        switch (operacao) {
            case '+':
                resultado = num1 + num2;
                break;

            case '-':
                resultado = num1 - num2;
                break;

            case '*':
                resultado = num1 * num2;
                break;

            case '/':
                if (num2 != 0) {
                    resultado = num1 / num2;
                } else {
                    System.out.println("Erro! Divisão por zero não é permitida.");
                    return;
                }
                break;

            default:
                System.out.println("Erro! Operação inválida.");
                return;
        }

        System.out.printf("O resultado é: %.2f", resultado);
    }
}
```
E retornou também algumas recomendações:

![retorno2](https://github.com/Hisly-A/DIO_IA_Generativa/assets/outputs/outputcopilot%2002.PNG)

Também é possível solicitar a geração de imagens, como no exemplo abaixo:

![solicitado2](https://github.com/Hisly-A/DIO_IA_Generativa/assets/inputs/inputcopilot%2002.PNG)

Para essa solicitação ele retornou as seguintes imagens:

![retorno3](https://github.com/Hisly-A/DIO_IA_Generativa/assets/outputs/outputcopilot%2003.PNG)

![retorno4](https://github.com/Hisly-A/DIO_IA_Generativa/assets/outputs/outputcopilot%2004.jpg)

![retorno5](https://github.com/Hisly-A/DIO_IA_Generativa/assets/outputs/outputcopilot%2005.jpg)
