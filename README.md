
# Aprendendo Docker 🐳

Este repositório é dedicado ao meu aprendizado sobre Docker. Estou explorando como construir imagens otimizadas, automatizar processos e utilizar boas práticas no desenvolvimento de containers. Atualmente, estou focando na **utilização de argumentos (ARG)** para gerar builds dinâmicos.

---

## 🚀 O que estou aprendendo

- **Dockerfile**: Estrutura básica, instruções e boas práticas.
- **Build com argumentos (ARG)**: Como utilizar variáveis para personalizar builds de forma eficiente.
- **Imagens otimizadas**: Técnicas para reduzir o tamanho das imagens Docker e aumentar a segurança.

---

## 🛠️ Como executar os exemplos

Certifique-se de ter o Docker instalado no seu ambiente. Para testar os exemplos deste repositório:

1. Clone o repositório:
   ```bash
   git clone (https://github.com/joaoalbuquerq/dockerTips.git)
   cd meuPrimeiroBuild
   ```

2. Construa a imagem utilizando argumentos:
   ```bash
   docker build --build-arg MEU_ARG=valor -t minha-imagem .
   ```

3. Execute o container:
   ```bash
   docker run minha-imagem
   ```

---

## 📝 Exemplos de uso de `ARG`

No meu aprendizado, implementei diferentes exemplos para explorar o uso de argumentos em builds. Aqui estão algumas ideias abordadas:

1. **Alterando variáveis em tempo de build**:
   ```dockerfile
   ARG MEU_ARG=valor-padrao
   ENV VAR_FINAL=$MEU_ARG
   ```

2. **Construindo com argumentos customizados**:
   ```bash
   docker build --build-arg MEU_ARG=customizado -t imagem-com-arg .
   ```

3. **Automatizando o build com múltiplos argumentos**:
   Exemplos de múltiplos argumentos podem ser encontrados [aqui](exemplo-multi-args).

---

## 📖 Recursos úteis

- [Documentação oficial do Docker](https://docs.docker.com/)
- [Boas práticas com Docker](https://docs.docker.com/develop/dev-best-practices/)
- [Explorando ARG e ENV](https://docs.docker.com/engine/reference/builder/#arg)

---

## 🌟 Próximos passos

- Aprender sobre **multi-stage builds**.
- Explorar o uso de **volumes** e **networks**.
- Criar um projeto prático com Docker Compose.

---

Contribuições e feedbacks são bem-vindos enquanto continuo aprendendo. Obrigado por acompanhar! 💻
