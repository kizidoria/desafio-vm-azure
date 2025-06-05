# desafio-vm-azure (Criação de Máquina Virtual no Azure)
desafio do bootcamp XP Inc. Cloud com Inteligência Artificial (DIO).
Este repositório contém a documentação e anotações sobre o processo de criação e configuração de uma **máquina virtual** no **Microsoft Azure**, como parte do bootcamp **XP Inc. Cloud com Inteligência Artificial**, oferecido pela **DIO (Digital Innovation One)**.
Aqui, você encontrará:
- Resumo do processo de criação da VM
- Dicas e melhores práticas para usar o Azure
- Capturas de tela das etapas do processo
- Passo a passo detalhado
Objetivo
O objetivo deste desafio foi praticar a criação e configuração de uma **máquina virtual** na plataforma Azure. A ideia é consolidar os conceitos aprendidos no bootcamp e criar um **material de referência** para futuras implementações.
## Passos Realizados
1. **Acesso ao portal do Azure**: Criação de conta ou login em `portal.azure.com`.
2. **Criação de grupo de recursos**: Para organizar as VMs e demais recursos.
3. **Configuração da máquina virtual**:
   - Escolha da **imagem** (Windows Server 2019 ou Ubuntu).
   - Escolha do **tamanho** da VM (ex: Standard B1s).
   - Configuração de **usuário e senha** para acesso.
4. **Configuração de rede**: Criação de regras de firewall para permitir **RDP (Windows)** ou **SSH (Linux)**.
5. **Provisionamento da VM**: Após a criação, a VM foi provisionada e ficou disponível para acesso.
## Dicas e Recomendações
- **Cuidado com os custos**: O Azure cobra por hora, então sempre desligue a VM quando não estiver utilizando.
- **Escolha da imagem**: Se possível, escolha uma imagem com suporte ao plano gratuito (por exemplo, `Ubuntu 20.04 LTS`).
- **Acesso remoto**: Para Windows, utilize o **RDP** (Remote Desktop Protocol). Para Linux, utilize o **SSH**.
- **Segurança**: Sempre crie regras de firewall para limitar o acesso à sua VM, evitando exposições desnecessárias.
- **Monitoramento**: Ative a opção de **alertas** de uso para garantir que não ultrapasse os limites de uso de recursos.
## Capturas de Tela
Abaixo estão as capturas de tela que ilustram as etapas principais do processo.
- **Configuração da VM no Azure**:
  ![Configuração da VM](./images/configuracao-vm.png)
- **Acesso via RDP**:
  ![Acesso via RDP](./images/acesso-rdp.png)
## Aprendizados
Durante o desenvolvimento do desafio, aprendi os seguintes pontos:
- **Azure Portal**: Familiarização com a criação e gerenciamento de máquinas virtuais no portal.
- **Computação em Nuvem**: Noções sobre a infraestrutura de nuvem, provisionamento de recursos e dimensionamento de VMs.
- **Segurança e Acesso**: Como configurar regras de firewall e acessar máquinas de forma segura.
## Links Úteis
- [Documentação Oficial do Azure - Criar uma VM](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal)
- [GitHub Markdown Guide](https://www.markdownguide.org/basic-syntax/)
- [Licença MIT](https://opensource.org/licenses/MIT)
## Como Rodar Localmente (para prática futura)
Após a criação da VM no Azure, você pode acessar a máquina remotamente:
### Para Windows:
- Use o **Remote Desktop Protocol (RDP)** para se conectar à VM:
  ```bash
  mstsc /v:<endereco-ip-da-vm>
