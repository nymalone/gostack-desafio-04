![Screen Shot 2020-06-24 at 14 40 26](https://user-images.githubusercontent.com/54912285/85605620-b59af580-b628-11ea-9c7a-f318a42dbba3.png)
<h1 align="center">
  🚀 Conceitos React Native 🚀
</h1>

#### If you need support with the content, go to my [Notion notes](https://www.notion.so/S01-Mobile-com-React-Native-7ffb8834ea074da8a18c1d96173c1299)
  
## 🚀 Desafio 03 
O objetivo deste desafio é colocar em prática os principais conceitos de React Native fazendo busca na api desenvolvida no [desafio 1](https://github.com/nymalone/gostack-desafio-01)

##  🤓 Conceitos importantes
### Principais diferenças com o ReactJS
Não vamos utilizar elementos do HTML. Temos que utilizar componentes que são exportados diretamente do pacote React Native, ex: **View** - div, footer, header, main, aside, section.

Os elementos do React Native não possuem valor semântico (significado), todos eles são usados de forma abstrata. Ex: **Text -** p, span, strong, h1, h2, h3...

Não possuem estilização própria. Ex h1 font-size 32px. **Tudo** precisa ser feito através de **CSS**.

Não vou criar arquivo **.css** a parte de css é feito dentro do código JS.

```jsx
const styles = StyleSheet.create({
    container: {
			flex: 1, 
        backgroundColor: "#7159c1",
				justifyContent: "center",
        alignItems: "center"
    },
		title: {
        color: "#fff",
        fontSize: 20,
        fontWeight: "bold",
    },
});
```

Todos componentes possuem por padrão **"display: flex"**  (por isso o flex 1 para ocupar a tela toda)

No React Native não temos ID ou ClassName, aqui nós vamos utilizar **style={styles.container}** 

```jsx
<View style={styles.container}>;
	<Text style={styles.title}> Hello GoStack </Text>
</View> 
```

No React Native não temos herança de estilos, então não adiantar eu colocar uma color: #fff dentro do container e esperar que o texto fique branco. Então preciso colocar um estilo especifico para cada tag.

### Funcionalidades da aplicação

- **`Listar os repositórios da sua API`**: Deve ser capaz de criar uma lista de todos os repositórios que estão cadastrados na sua API com os campos **title**, **techs** e número de curtidas seguindo o padrão `${repository.likes} curtidas`, apenas alterando o número para ser dinâmico.

- **`Curtir um repositório listado da API`**: Deve ser capaz de curtir um item na sua API através de um botão com o texto **Curtir** e deve atualizar o número de likes na listagem no mobile.

### Específicação dos testes

Para esse desafio temos os seguintes testes:

- **`should add a like to the like counter of the repository`**: Para que esse teste passe, sua aplicação deve permitir ao clicar no botão `Curtir`, um like seja adicionado ao repositório listado, e que essa atualização possa ser visualizada na tela.

***

<h4 align="center">
    Made with :coffee: and 💜 by <a href="https://www.linkedin.com/in/nykollemalone/" target="_blank">Nykolle Malone</a>
</h4>

