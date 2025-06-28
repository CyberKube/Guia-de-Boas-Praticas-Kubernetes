# 📘 Guia de Boas Práticas para Segurança da API do Kubernetes

Este repositório contém um conjunto de boas práticas para fortalecer a segurança da API do Kubernetes, com foco em ambientes críticos, como cidades inteligentes. O conteúdo foi desenvolvido com base em testes práticos realizados em um cluster local com Minikube e está alinhado às recomendações de segurança modernas para clusters Kubernetes.

---

## 📑 Estrutura do Guia

O guia está dividido nos seguintes tópicos:

1. **Introdução**  
   Visão geral e motivação para aplicação de boas práticas em segurança de APIs Kubernetes.

2. **Autenticação e Autorização**  
   - Implementação de autenticação forte (Tokens, TLS 1.3)  
   - Configuração de RBAC com base no menor privilégio

3. **Proteção de Secrets**  
   - Armazenamento seguro  
   - Criptografia em repouso (etcd)  
   - Acesso restrito via RBAC

4. **Proteção TLS e HTTPS**  
   - Exigência de TLS 1.3  
   - Certificados válidos (Let's Encrypt, self-signed)  
   - Validação e rotação de certificados

5. **Controle de Acesso à API**  
   - Bloqueio de exposição direta  
   - Uso de VPN, firewalls e Ingress com TLS  
   - Restrições por IP e rate limiting

6. **Ferramentas e Auditoria**  
   - Falco, Kubeaudit, cert-manager  
   - Postman com token JWT para testes controlados

7. **Pontos de Atenção**  
   - Riscos associados à ausência de MFA, controle por IP e limitação de requisições

8. **Conclusão**  
   Segurança como processo contínuo: necessidade de revisão e atualização constantes.

---

## 🛠 Ferramentas Utilizadas

- [Minikube](https://minikube.sigs.k8s.io)
- [kubectl](https://kubernetes.io/docs/reference/kubectl/)
- [Falco](https://falco.org/)
- [Kubeaudit](https://github.com/Shopify/kubeaudit)
- [cert-manager](https://cert-manager.io)
- [Postman](https://www.postman.com/)

---

## 📂 Arquivos Disponíveis

- `Guias-de-boas-praticas.pdf`: Documento completo com todas as boas práticas.
- `roadmap.png`: Roadmap visual contendo os principais tópicos do guia.
- Exemplos de arquivos YAML para RBAC, Secrets e TLS (em breve).

---

## 📎 Repositório Oficial

Todo o conteúdo pode ser acessado, atualizado e reutilizado a partir do repositório:

🔗 [https://github.com/CyberKube/Guia-de-Boas-Praticas-Kubernetes](https://github.com/CyberKube/Guia-de-Boas-Praticas-Kubernetes)

---

## 👥 Autores

Projeto desenvolvido como parte do Trabalho de Conclusão de Curso da FATEC São Caetano do Sul (2024):

- Arthur Nolasco  
- Ian Guimarães
- Marcelo Augusto Andrade da Silva
- Michele Bueno  
- Rafael Nascimento

---

## 📄 Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.
