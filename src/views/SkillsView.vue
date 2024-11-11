<template>
  <div class="skills">
    <div class="section">
        <h2>O que faço?</h2>
        <ul>
            <li v-for="(item, i) in list_skills" :key="i">{{ item }}</li>
        </ul>
    </div>
  </div>
</template>
<script setup>
  const list_skills = [
    "Administro soluções de segurança (Proxy, Firewall, IDPS)",
    "Analiso indicadores e identifico oportunidades de melhorias na infraestrutura de TI",
    "Automatizo deploy de Máquinas Virtuais",
    "Desenvolvo playbooks Ansible para gerir dispositivos de rede (routers, switches, firewalls)",
    "Elaboro e implemento políticas de roteamento interno e externo",
    "Especifico requisitos técnicos para aquisição de dispositivos e soluções de redes e segurança",
    "Implemento e gerencio serviços de rede em servidores Linux e Windows",
    "Ministro capacitações técnicas para equipes internas e de clientes"
  ]
</script>
