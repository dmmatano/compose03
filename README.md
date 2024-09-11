# Compose 03

### State
Qualquer valor que pode mudar ao longo do tempo. Ou melhor, determina o que é mostrado na tela em determinado momento.
Ao atualizar um state, ocorre a "recomposition", isto é, o composable relacionado ao state é "recarregado".
Usamos remember para evitar que a variavel seja "resetada" na hora do recomposition.
O uso do remember não funciona em mudanças de configuração do dispositivo (landscape, idioma, etc). Utilize rememberSaveable.
<br>
Stateless Composable: não possui nenhum state. Não guarda, cria ou modifica nenhum state.<br>
Statefull Composable: possui uma parte do state.<br>
Quando fazer o "hoist" de um state:
- O state deve fazer o hoist pelo menos ao pai comum mais baixo de todos os composables que usam o state (read).
- O state deve fazer o hoist pelo menos ao nível mais alto, podendo ser alterado (write).
- Se dois state mudam em resposta aos mesmos acontecimentos, devem ter um hoist ao mesmo nível.
<br>


