

# Linux Fixes (Pop!_OS) 🐧

Coleção de scripts para corrigir problemas comuns de áudio (chiado no microfone) e conexões Bluetooth no Linux. 

> **Nota:** Estes scripts foram testados e criados com base no **Pop!_OS**. Podem funcionar em outras distros baseadas em Debian/Ubuntu, mas sem garantia.

## 🐧 Sobre o repositório:

> Siga as instruções abaixo para configurar o ambiente e rodar os scripts.

### Pré-requisitos

Para utilizar a correção de microfone, utilizaremos o **NoiseTorch**. É necessário ter o `git` e o compilador `golang` instalados:

```bash
sudo apt update
sudo apt install golang git -y

```

### Instalação e Configuração

#### 1. Permissões de Execução

Dê permissão de execução para os scripts baixados:

```bash
chmod +x bluet.sh
chmod +x mic.sh

```

#### 2. Configurando o NoiseTorch (Microfone)

Este passo compila e instala a ferramenta de supressão de ruído:

```bash
# Baixa o repositório
git clone https://github.com/noisetorch/NoiseTorch
cd NoiseTorch

# Compila o projeto
make

```

## 🛠️ Como Usar

Para rodar manualmente:

```bash
./bluet.sh
# ou
./mic.sh

```

### Automatizando (Opcional)

Para não precisar rodar toda vez que ligar o PC, adicione o caminho do script no aplicativo **"Aplicativos de Inicialização"** (Startup Applications) do Pop!_OS.

## 📄 Créditos e Referências

* Soluções baseadas em discussões do Reddit e Fóruns Linux.
* Ferramenta de áudio: [NoiseTorch](https://github.com/noisetorch/NoiseTorch)

>Divirta-se! :)
