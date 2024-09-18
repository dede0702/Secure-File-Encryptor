# Secure-File-Encryptor

Aqui está um modelo de README para o seu projeto de criptografia de arquivos em Python:

---

### Descrição
O **Secure File Encryptor** é uma ferramenta desenvolvida em Python para garantir a proteção de arquivos sensíveis, utilizando o protocolo AES (Advanced Encryption Standard). A aplicação permite criptografar e descriptografar arquivos de uma pasta específica, garantindo que apenas usuários com a senha correta tenham acesso ao conteúdo dos arquivos. Além disso, o sistema gera backups criptografados dos arquivos em uma nova pasta.

### Funcionalidades
- **Criptografia AES**: Utiliza o protocolo AES (Fernet) para garantir segurança na criptografia dos arquivos.
- **Descriptografia Segura**: Permite descriptografar arquivos previamente criptografados, garantindo acesso apenas com a senha correta.
- **Backup Automático**: Cria uma nova pasta com os arquivos criptografados como backup.
- **Fácil Integração**: Permite integrar a solução em qualquer sistema ou fluxo de trabalho.

### Estrutura do Projeto
1. **Entrada da senha**: O usuário fornece uma senha que será usada para derivar a chave de criptografia.
2. **Acesso à pasta**: O programa acessa a pasta com os arquivos que devem ser criptografados.
3. **Criptografia dos arquivos**: Todos os arquivos são criptografados usando AES.
4. **Backup dos arquivos**: Os arquivos criptografados são salvos em uma nova pasta.
5. **Descriptografia dos arquivos**: O sistema permite a descriptografia dos arquivos, garantindo que a senha correta seja usada.

### Requisitos
- Python 3.6 ou superior
- Biblioteca `cryptography`

### Instalação
1. Clone o repositório:

   ```bash
   git clone https://github.com/usuario/secure-file-encryptor.git
   ```

2. Instale as dependências necessárias:

   ```bash
   pip install cryptography
   ```

### Como Usar
1. Execute o script principal do projeto:

   ```bash
   python encryptor.py
   ```

2. Informe a senha para criptografia e a pasta contendo os arquivos que deseja criptografar.
3. O programa criará automaticamente uma nova pasta contendo os arquivos criptografados.
4. Para descriptografar, execute o programa novamente e siga as instruções para inserir a senha correta.

### Exemplo de Uso

#### Criptografar Arquivos
```bash
Digite sua senha para criptografia: ********
Arquivos da pasta 'original/' criptografados e salvos em 'backup/'.
```

#### Descriptografar Arquivos
```bash
Digite sua senha para descriptografia: ********
Arquivos descriptografados e restaurados para 'original/'.
```

### Estrutura de Pastas
```
/secure-file-encryptor
  ├── encryptor.py       # Script principal
  ├── README.md          # Documentação do projeto
  └── requirements.txt   # Dependências do projeto
```

### Licença
Este projeto está licenciado sob a [MIT License](LICENSE).

---

