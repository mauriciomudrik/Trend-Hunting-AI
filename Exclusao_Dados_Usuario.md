# Exclusão de Usuário

---

## 🇧🇷 Português: O que acontece ao excluir um usuário?

Ao solicitar a exclusão de um usuário através do painel de administração, você tem à disposição as seguintes opções para gerenciar os dados vinculados a essa conta:

1. **Fazer backup e enviar para o e-mail do usuário**:
   - O sistema irá compilar todos os dados do usuário, assim como os dados dos projetos em que ele é o único dono, incluindo posts coletados, métricas e chaves.
   - Um arquivo JSON estruturado contendo essas informações será enviado automaticamente em anexo para o e-mail cadastrado deste usuário.

2. **Remover todos os dados relacionados (projetos, posts, configurações de API e OAuth)** (Deep Wipe):
   - Se esta opção estiver marcada, não apenas o usuário será removido. O sistema apagará permanentemente todos os projetos em que este usuário seja o membro exclusivo.
   - Isso garante o encerramento imediato de coletas (posts), chaves de API (Configurações API) e sessões de OAuth ou scraping ativas cadastradas sob a conta do usuário nesses projetos.
   - **Auditoria de Exclusão (Log)**: Sempre que esta ação profunda for executada, a API do sistema criará internamente um arquivo de texto com o log detalhado. Este log listará cada projeto excluído, além de descrever cada chave de API ou de OAuth removida, permitindo conformidade e ratificando a exclusão dos ativos digitais confidenciais.
