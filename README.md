# Painel CLT — tela de acesso

Esta é só a porta de entrada do Painel CLT (Grupo N1 e Grupo Multiplique).
Nenhum número fica aqui: depois da senha, a página busca o painel e os dados no banco, por funções que só leem as consultas fixas do painel.

- A senha fica guardada no banco só como resumo (bcrypt); ninguém consegue lê-la.
- A sessão vale 12 horas; depois disso a página pede a senha de novo.
- A chave que aparece no `index.html` é a chave pública do Supabase, feita para ficar em página: sozinha ela não lê nenhum dado.
