Sua base já está ótima! Eu ajustei pequenos pontos para melhorar a clareza, deixei o passo a passo mais direto e padronizei a formatação. Aqui vai a versão **melhorada**:

````markdown
# 📊 Grafana GIFs Repository

Este repositório é utilizado para armazenar **GIFs** que são usados nos **dashboards do Grafana**, através de **HTML customizado** 🎯.  
A ideia é manter todos os GIFs organizados e versionados para facilitar a personalização visual dos painéis.

## 🚀 Como Usar no Grafana

1. Faça upload dos GIFs no servidor ou em um serviço como **Imgur**.
2. No painel do Grafana, adicione um painel com visualização do tipo **Business Text**.
3. Em **Select Editors to display. Editors with updated values always displayed**, selecione **Styles** para habilitar o uso de CSS.
4. Em **Content**, insira o seguinte código HTML:

   ```html
   <div id="main">
     <img src="https://i.imgur.com/sSw5MDy.gif" alt="GIF">
     <div id="texts">
       <span class="values">{{value}}%</span>
       <span class="label">Uso de disco</span>
     </div>
   </div>
    ```

5. Em **CSS Styles**, insira o seguinte código CSS:

   ```css
   * {
     margin: 0;
     padding: 0;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
     box-sizing: border-box;
   }

   #main {
     display: flex;
     justify-content: space-between;
     align-items: center;
     background: linear-gradient(135deg, #003366, #0E1838);
     padding: 10px 10px;
     border-radius: 16px;
     box-shadow: 0 6px 15px rgba(0, 0, 0, 0.25);
     color: white;
   }

   #main img {
     height: 50px;
     border-radius: 8px;
   }

   #texts {
     display: flex;
     flex-direction: column;
     align-items: flex-start;
     line-height: 1.2;
   }

   .values {
     font-size: 2.2rem;
     font-weight: 600;
   }

   .label {
     font-size: 1rem;
     opacity: 0.7;
   }
   ```

6. Ajuste a **URL do GIF** e os textos conforme necessário para o seu painel.

## 📦 Regras para Contribuição

* Somente GIFs otimizados e leves (preferencialmente abaixo de 2MB).
* Nomeie os arquivos de forma descritiva e use `-` para separar palavras (exemplo: `server-down.gif`).
* Mantenha a raiz do repositório limpa, sem subpastas.

## 💡 Dicas

* Use ferramentas como [ezgif.com](https://ezgif.com/) para redimensionar e otimizar seus GIFs antes de adicioná-los aqui.
* Para hospedar seus GIFs de forma simples, utilize serviços como:

  * [Imgur](https://imgur.com/)
  * [Postimages](https://postimages.org/)