# Compose 03

### State
Qualquer valor que pode mudar ao longo do tempo. Ou melhor, determina o que é mostrado na tela em determinado momento.
Ao atualizar um state, ocorre a "recomposition", isto é, o composable relacionado ao state é "recarregado".
Usamos remember para evitar que a variavel seja "resetada" na hora do recomposition.
O uso do remember não funciona em mudanças de configuração do dispositivo (landscape, idioma, etc). Utilize rememberSaveable.

<br>


