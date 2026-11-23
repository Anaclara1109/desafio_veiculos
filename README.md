Cadastro de Veículos (Dart + Supabase)

Professor(a), este projeto é um cadastro de veículos no terminal. Dá para cadastrar, listar, atualizar e excluir veículos, e os dados ficam salvos no Supabase.

Como configurar a conexão
Criar a tabela: no Supabase, abra o SQL Editor, cole o conteúdo do arquivo schema.sql e clique em Run.
Criar o .env: na raiz do projeto, copie o .env.example para .env e preencha:
SUPABASE_URL=https://supabase.com/dashboard/project/cwgjxnkhfrmqtydqkffe/settings/api-keys
SUPABASE_PUBLISHABLE_KEY=sb_publishable_-adw1AXEyMiZMbRID8fkuA_2AiLiohI

A URL e a chave estão em Settings > API Keys no painel do Supabase. O .env não foi enviado ao GitHub, por isso precisa ser criado.

Instalar as dependências:
dart pub get
Como executar

Na raiz do projeto:

dart run bin/main.dart

O menu aparece e o programa continua até escolher a opção 0.

Arquivos
bin/main.dart: menu, leitura e validação das entradas.
lib/conexao.dart: carrega o .env e conecta ao Supabase.
lib/veiculos.dart: métodos do CRUD.
schema.sql: cria a tabela e as permissões.
