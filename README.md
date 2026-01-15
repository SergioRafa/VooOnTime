

✈️ VooOnTime - Dashboard Preditivo de Atrasos
O VooOnTime é uma solução Full-Stack que utiliza Inteligência Artificial para prever a probabilidade de atrasos em voos comerciais brasileiros em tempo real. O sistema integra dados climáticos reais, monitorização de tráfego aeroportuário e um modelo de Machine Learning treinado.

🚀 Arquitetura do Sistema
A nossa solução utiliza uma arquitetura híbrida e distribuída:

Frontend (GitHub Pages): Interface responsiva em HTML5/CSS3, acessível de qualquer dispositivo.

Orquestrador Backend (Java / Spring Boot): Responsável por consumir APIs externas, tratar as regras de negócio e comunicar com o motor de IA.

Motor de Inteligência Artificial (Python / Flask): Modelo de Machine Learning que processa as variáveis e calcula a probabilidade de atraso.

Túnel de Comunicação (Ngrok): Garante a conectividade segura entre o frontend na nuvem e os servidores locais.

🧠 Inteligência de Dados e Integrações
O sistema não utiliza dados estáticos. Para cada análise, consultamos:

StormGlass API: Dados meteorológicos reais (temperatura, velocidade do vento) com base nas coordenadas do aeroporto.

News API / Traffic Monitor: Monitorização de incidentes e tráfego crítico nos principais hubs aéreos.

🛠️ Tecnologias Utilizadas
Linguagens: Java 17, Python 3.9, JavaScript.

Frameworks: Spring Boot, Flask, Scikit-Learn.

DevOps & Cloud: GitHub Pages, Git, Ngrok.

📊 Cenários de Validação
Aeroporto	Condições Climáticas	Tráfego	Risco Calculado
Manaus (MAO)	28.1°C / Vento 12.7km/h	Normal	20% (Baixo)
Guarulhos (GRU)	28.1°C / Vento 12.7km/h	Crítico	85% (Alto)
