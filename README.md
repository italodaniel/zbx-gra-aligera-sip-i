# zbx-gra-aligera-sip-i

Media Gateway Aligera AG1700 SIP-I
Template Zabbix e Dashboard Grafana
OBS: Nos prints em anexo foi removido os IPs na coleta do SIP PEERS HOSTS por questões de segurança.

## PT-BR
Template_Aligera_AG1700_SIP-I e Grafana Dashboard

**Zabbix**: [Repositório no GitHub](https://github.com/italodaniel/zbx-gra-aligera-sip-i)

**Grafana**: [Dashboard no Grafana](https://grafana.com/grafana/dashboards/20086-sip-i-tim-brasil/)

### HOMOLOGADO PARA:
- Zabbix 6.4.8
- Grafana 10.2.2

MIB Aligera: [Link para download](https://docs.aligera.com.br/images/b/b5/ALIGERA-MIB.mib)

### PASSOS:

#### No Zabbix:
1. Crie um grupo chamado **Aligera**.
2. Importe o template **Aligera-SIP-I** atribuindo-o ao grupo **Aligera** no Zabbix. (Essa organização foi mantida para melhor experiência, mas fique à vontade para ajustar conforme necessário).
3. No Hostgroup, use o nome "Aligera_SIP_GWM_TIM" e vincule o modelo ao host. Esse hostname foi utilizado para o modelo de coleta de interconexão.
4. Para a interface, utilize o tipo SNMP e informe o IP do Aligera.
5. Atribua o template importado ao host.
6. Aguarde a coleta de dados ou utilize a função "Verificar agora" no item e no LLD para acelerar a coleta.

#### No Grafana:
Importe o Dashboard: [SIP-I - ALIGERA - Dashboard](https://grafana.com/grafana/dashboards/20086-sip-i-tim-brasil/). Com o template já importado, selecione a Fonte de Dados, que é o Zabbix.
1. Ao selecionar a query, siga a ordem do print em anexo.
2. Item - PeersNameOne, PeersHostOne e KeepaliveOne. 
3. Os itens devem seguir a ordem numérica conforme mencionado acima.

### Dúvidas e sugestões de melhoria:
- Instagram: [daniel_itallo](https://www.instagram.com/daniel_itallo)
- Linkedin: [Daniel Italo](https://www.linkedin.com/in/daniel-italo/)
- Telegram: @daniel_itallo

![image](https://github.com/italodaniel/zbx-gra-aligera-sip-i/assets/47395906/f0c25fc6-4170-400e-b470-e22bfa245ea8)


  
