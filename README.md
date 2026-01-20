✈️ VooOnTime: Ecossistema Preditivo de Resiliência AéreaO VooOnTime é uma solução Full-Stack de alta disponibilidade que utiliza Inteligência Artificial para transformar dados brutos em previsibilidade. O sistema antecipa a probabilidade de atrasos em voos comerciais brasileiros, integrando variáveis climáticas, geolocalização e fluxos de tráfego terrestre em tempo real.

🚀 Arquitetura de MicroserviçosNossa solução rompe o modelo monolítico e utiliza uma arquitetura híbrida e distribuída para garantir performance:Frontend (UX Edge): Interface responsiva hospedada via GitHub Pages, projetada com foco em Zero Friction (sem necessidade de login) e acessibilidade universal.Orquestrador (Java / Spring Boot): O núcleo da aplicação. Gerencia o consumo de APIs externas, aplica regras de negócio e atua como o gateway seguro para o motor de IA.Motor de Inferência (Python / Flask): Modelo de Machine Learning (Scikit-Learn) que processa variáveis complexas para gerar predições probabilísticas instantâneas.Conectividade (Ngrok Tunneling): Implementação de túnel seguro para comunicação entre a interface cloud e o processamento local, simulando um ambiente de produção real.

🧠 Inteligência de Contexto e ResiliênciaDiferente de soluções estáticas, o VooOnTime opera em tempo real com mecanismos de segurança:Data Sourcing: Integração ativa com StormGlass API (clima) e News/Traffic Monitor (incidentes).Mecanismo de Fallback: Sistema inteligente que detecta falhas em APIs externas (como erros 403 de limite de cota) e aciona automaticamente um módulo de simulação heurística para manter a aplicação online.

🛠️ Stack TecnológicaLinguagens: Java 17+, Python 3.9+, JavaScript (ES6+).Frameworks: Spring Boot (Ecossistema Spring), Flask, Scikit-Learn.Infraestrutura: Git, GitHub Actions, Ngrok.

📊 Validação e Resultados (Logs de Produção)O modelo demonstra alta sensibilidade ao fator humano/terrestre, não apenas ao clima:

Aeroporto,Temperatura / Vento,Fluxo de Tráfego,Risco IA,Status
Manaus (MAO),31.2°C / 4.5km/h,Fluxo Normal,20%,✅ Pontual
Curitiba (CWB),17.5°C / 14.2km/h,Fluxo Normal,20%,✅ Pontual
Guarulhos (GRU),24.5°C / 8.0km/h,CONGESTIONAMENTO,85%,⚠️ Risco Alto

Nota Técnica: Observe que em Guarulhos, mesmo com condições climáticas favoráveis, o sistema identificou o tráfego crítico na Rod. Hélio Smidt, elevando o risco para 85%. Isso comprova a eficácia da nossa análise multivariável.
