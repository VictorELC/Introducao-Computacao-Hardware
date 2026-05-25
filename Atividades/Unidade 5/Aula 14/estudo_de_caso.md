# Stuxnet - Estudo de Caso

## Contexto do ataque.

O Stuxnet é um malware que ficou famoso por ter sido usado para atacar instalações iranianas, quando foi descoberto em 2010. Foi descoberto quando inspetores visitantes da agência de Energia Atômica viram várias centrífugas falhando. Era difícil acreditar que era um malware o responsável, pois as instalações nucleares do Irã não estavam conectadas a uma rede ou à internet. Quando uma equipe de segurança bielorrussa foi investigar o mau funcionamento dos computadores da instalação, foi descoberto esse malware altamente complexo. Até hoje não se sabe com 100% de certeza quem criou esse software, mas acredita-se que foi criado pelos EUA com auxílio de Israel, com o objetivo de deter ou atrasar o programa nuclear iraniano, por meio de um pen drive comprometido na rede própria da usina.

E apesar de ser um malware, não é um vírus, mas um worm de computador, ou seja, um malware autônomo e independente, capaz de se autorreplicar e se espalhar automaticamente por redes, sem necessidade de interação humana, lembrando muito um vírus biológico.

## Vulnerabilidades exploradas

O Stuxnet tinha um código muito complexo, e funcionava infectando os controladores lógicos programáveis (CLPs) que controlavam as centrífugas, e sabotando-as.
Ele utilizava vulnerabilidades de dia zero desconhecidas no sistema operacional Windows para pular de um computador para outro, utilizando-os como uma ponte para chegar ao objetivo final, que eram os softwares que controlavam as  centrífugas, para alterar os CLPs e fazendo as centrífugas girarem por muito tempo muito rápido, e simultaneamente enviava dados falsos para fazer parecer que tudo funcionava normalmente.

## Impactos

O Stuxnet conseguiu destruir quase um quinto das centrífugas nucleares do Irã, e infectou mais de 200.000 computadores, causando degradação física de 1000 máquinas. Além do impacto direto nas instalações iranianas, o Stuxnet alterou o panorama de cibersegurança, destacando vulnerabilidades em infraestruturas críticas, forçando organizações e governos a repensar as estratégias de cibersegurança. Mas o maior impacto do Stuxnet foi o sentimento de insegurança na sociedade

## Medidas de mitigação

Aplicação de políticas rigorosas de BYOD, ou Bring Your Own Device;
Air gap de qualquer computador que possa afetar a segurança nacional;
Aplicação de backup e restauração fácil em todos os níveis possíveis para minimizar a  interrupção, aplicação de tecnologias, e a prática dos fundamentos básicos de higiene cibernética, mantendo o sistema operacional e o software de segurança atualizados, visto que as vulnerabilidades de dia zero já foram corrigidas há muito tempo.
