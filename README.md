SOBRE O PROJETO:

O projeto simula a requisição de um profissional contratado para implementar uma rede em uma clínica médica. A rede deve estar funcional e todos os dispositivos devem acessar a Internet e compartilhem arquivos entre si. Foram considerados 3 computadores (Recepção, Consultório 1 e Consultório 2) e 1 impressora de rede.   


OBJETIVO: 

Implementar a rede, fazer os dispositivos acessarem a internet e compartilhar arquivos entre si, escolher os equipamentos corretos, definir a topologia e criar um diagrama lógico da rede.



SOFTWARE UTILIZADO: Cisco Packet tracer.



INFRAESTRUTURA - JUSTIFICATIVA:

Os equipamentos utilizados para executar o projeto foram: roteador, switch e cabo.

A escolha do Switch (camada de enlace) se deve a sua diferença em relação ao hub. O switch funciona como um organizador na rede local que identifica o destinatário correto e envia os dados diretamente para ele.O uso do switch minimiza colisões e reduz o tráfego desnecessário. Além disso, os hubs tornaram-se obsoletos em muitos cenários e foram amplamente superados pelos switches, que oferecem melhor controle e performance para as redes contemporâneas. Outro aspecto é a segurança**.** Ao não replicar os dados para todas as máquinas da clínica, o switch garante que as informações de um consultório não circulem desnecessariamente nos outros computadores.

O Roteador, por atuar como um "diretor de tráfego", ficou responsável por conectar redes diferentes (como a sua rede local e a rede mundial de computadores) e direcionar os pacotes de dados entre elas(camada de rede). Para isso, o roteador trabalha em conjunto com um Modem, que é o aparelho que transforma os sinais digitais da rede local em sinais que podem viajar pelas linhas do provedor.



TOPOLOGIA - DESCRIÇÃO:

A topologia utilizada neste projeto foi do tipo estrela, pois, oferece as seguintes vantagens:

Isolamento de falhas: Caso ocorra um problema no cabo de um dos computadores dos consultórios, apenas aquela conexão é afetada, enquanto o restante da clínica continua operando normalmente.

Facilidade de gerenciamento: É simples adicionar ou remover dispositivos (como uma nova impressora ou computador) sem interromper a rede.

Organização centralizada: Todos os dispositivos se conectam a um ponto central (o switch), que organiza a comunicação de forma eficiente.

Além disso, a topologia estrela é a configuração padrão mais utilizada em escritórios e ambientes profissionais modernos devido à sua robustez e praticidade.





TABELA DE ENDEREÇAMENTO IP (IPV4)



|Identificação do Dispositivo|Interfaces de Rede|Endereço IP|Máscara de Sub-rede|Gateway Padrão (Default Gateway)|Servidores DNS|
|-|-|-|-|-|-|
|Consultorio\_1|FastEthernet0/0|192.168.1.1|255.255.255.0|192.168.0.254|-|
|Consultorio\_1|FastEthernet0/0|192.168.1.2|255.255.255.0|192.168.0.254|-|
|Impressora|FastEthernet0/0|192.168.1.4|255.255.255.0|192.168.0.254|-|
|Recepcao|FastEthernet0/0|192.168.1.3|255.255.255.0|192.168.0.254|-|
|Roteador|FastEthernet0/0|192.168.0.254|-|192.168.0.254|-|
|Switch|FastEthernet0/0|-|-||-|















