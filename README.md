UNIQUELAB7 - Website Institucional

O website da UNIQUELAB7 é uma plataforma institucional desenvolvida para apresentar a estrutura, os serviços e os diagnósticos laboratoriais oferecidos pela empresa. O projeto prioriza uma navegação intuitiva, alta performance e um design adaptável para diferentes dispositivos, visando transmitir a precisão e a tecnologia do laboratório de análises clínicas.

Sumário

Visão Geral

Áreas de Atuação

Funcionalidades

Tecnologias Utilizadas

Estrutura do Projeto

Configuração do Ambiente e Execução

Integração e Segurança com Firebase

Internacionalização

Status e Licença

Visão Geral

A plataforma atua como ponto central de contato para pacientes, clínicas, hospitais e parceiros corporativos. O desenvolvimento focou em proporcionar uma experiência fluida, acessível e segura, unindo apresentação institucional e canal direto para atendimento.

Áreas de Atuação

O catálogo de exames e serviços abrange as seguintes especialidades laboratoriais:

Hematologia

Química Clínica

Microbiologia

Imunologia

Biologia Molecular

Urinálise

Exames Toxicológicos

Soluções Corporativas e Parcerias

Funcionalidades

Design Responsivo: Layout adaptado para desktop, notebooks, tablets e dispositivos móveis utilizando os breakpoints do Tailwind CSS.

Internacionalização (i18n): Suporte nativo para múltiplos idiomas (Português, Inglês e Espanhol) configurável diretamente pela interface.

Acessibilidade e SEO: Estruturação orientada a SEO com metadados detalhados, suporte a navegação por teclado e dados estruturados via Schema.org.

Painel Administrativo: Interface dedicada para gerenciamento de dados e informações do projeto.

Integração Comercial: Canal de contato direto integrado via WhatsApp.

Performance: Animações e navegação otimizadas para carregamento rápido.

Tecnologias Utilizadas

Front-end: HTML5, CSS3, JavaScript (ES6+)

Estilização: Tailwind CSS

Backend e Serviços: Firebase (Authentication, Firestore/Realtime Database, Hosting)

Recursos Adicionais: Google Fonts, Schema.org

Estrutura do Projeto

uniquelab7/
│
├── index.html       # Página principal com apresentação institucional e serviços
├── admin.html       # Painel administrativo de gerenciamento
├── README.md        # Documentação do projeto
└── .gitignore       # Arquivos e diretórios ignorados pelo Git


Configuração do Ambiente e Execução

Pré-requisitos

Para executar o projeto localmente, é necessário apenas um navegador web e um servidor HTTP simples.

Passo a Passo

Clonar o repositório:

git clone https://github.com/usuario/uniquelab7.git


Acessar o diretório do projeto:

cd uniquelab7


Executar o servidor local:
Utilizando Python (versão 3.x):

python -m http.server 5500


Alternativamente, utilize a extensão Live Server no VS Code.

Acessar no navegador:
Abra o endereço http://localhost:5500 no seu navegador.

Integração e Segurança com Firebase

O projeto consome serviços do Firebase para gerenciamento de dados. Para garantir a integridade da aplicação e seguir as boas práticas de segurança:

Credenciais e Segredos: Nunca comite credenciais privadas, arquivos .env ou chaves de serviço (serviceAccountKey.json).

Exemplo de Configuração Pública (firebaseConfig):

const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_AUTH_DOMAIN",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_STORAGE_BUCKET",
    messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
    appId: "YOUR_APP_ID",
    measurementId: "YOUR_MEASUREMENT_ID"
};


Regras de Acesso: Certifique-se de configurar as regras de segurança do Firebase (Security Rules) no console para restringir acessos não autorizados, especialmente nas rotas do painel administrativo (admin.html).

Exemplo de .gitignore recomendado para o ambiente:

.env
.env.local
.env.production
*.key
*.pem
serviceAccount.json
firebase-adminsdk*.json


Internacionalização

O suporte a idiomas no site é estruturado para atender aos seguintes parâmetros:

pt-BR: Português (Brasil) - Idioma padrão

en-US: Inglês

es-ES: Espanhol

A troca de idioma altera dinamicamente os textos da interface preservando a estrutura da página.

Status e Licença

Status do Projeto

O projeto encontra-se em desenvolvimento contínuo, passando por otimizações frequentes de código, segurança e melhorias na experiência do usuário.

Créditos

Desenvolvido por João Pedro Diniz para a UNIQUELAB7.

Licença

Este software é proprietário e de uso exclusivo da UNIQUELAB7. A cópia, distribuição ou modificação não autorizada de seu código, identidade visual ou conteúdos é estritamente proibida.
