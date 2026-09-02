::: step
#### Desativar Checkpoints Automáticos
*Configuração única por VM*
Evita que o Hyper-V gere novos arquivos diferenciais ao ligar/desligar.
- No Gerenciador do Hyper-V, acesse Configurações da VM > Gerenciamento > Pontos de Verificação.
- Desmarque a opção Habilitar pontos de verificação automáticos.
- Alternativa via PowerShell no Host:
```powershell
Set-VM -Name "NomeDaVM" -AutomaticCheckpointsEnabled $false
```
:::
::: step
#### Excluir Árvore de Checkpoints
*2.Excluir Árvore de Checkpoints:Pré-requisito para liberar o VHDX base.*
Mescla as alterações de volta ao disco principal para destravar a edição do arquivo.
- Na seção inferior de Pontos de Verificação, clique com o botão direito no ponto raiz e selecione Excluir Subárvore de Ponto de Verificação.
- Aguarde o Hyper-V finalizar a mesclagem dos arquivos .avhdx no painel de status.  
:::
::: step
#### Executar ReTrim dentro da VM
*Executar no Guest*
Informa ao sistema de arquivos quais setores foram apagados para que possam ser zerados.  
- Ligue a VM e abra o PowerShell como Administrador dentro dela:
``` powershell
Optimize-Volume -DriveLetter C -ReTrim -Verbose
```
- (Para VMs Linux, o equivalente no terminal é sudo fstrim -av).
:::
::: step
#### Desligar a VM Completamente
*Não utilize 'Salvar Estado'*
O disco virtual não pode ter nenhum lock de leitura/escrita durante a compactação no host.  
- Execute o desligamento limpo diretamente pelo sistema operacional da VM.
:::
::: step
#### Executar Otimização no Host
*PowerShell como Administrador no Windows Host*
Monta o disco em modo somente leitura e recolhe o espaço físico livre do arquivo .vhdx.
``` powershell
Mount-VHD -Path "C:\Caminho\Do\SeuDisco.vhdx" -ReadOnly
Optimize-VHD -Path "C:\Caminho\Do\SeuDisco.vhdx" -Mode Full
Dismount-VHD -Path "C:\Caminho\Do\SeuDisco.vhdx"
```
:::
::: step-last
#### Validar e Criar Ponto Manual Limpo
*Opcional*
- Inicie a VM e confirme se os serviços e dados estão íntegros.
- Execute o desligamento limpo diretamente pelo sistema operacional da VM.
- No gerenciador do Hyper-V clique com o botão direito do mouse sobre a VM e selecione `Ponto de Verificação`.
- Confiorme na aba inferior chamada `Ponto de verificação` que o ponto foi criado.
:::
