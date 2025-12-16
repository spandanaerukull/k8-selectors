Kubernetes Scheduling & Placement Strategies
This repo contains concise, example-driven YAML files that simplify key Kubernetes concepts: node and pod placement using selectors, affinity/anti-affinity rules, and real-world scheduling logic. Ideal for interview prep or visual explanations in content creation.

📁 File Breakdown
📄 Filename	🔍 Purpose
01-node-selector.yaml	🎯 Assign pods to nodes with explicit labels using nodeSelector
02-node-selector.yaml	🧪 Variant example to reinforce nodeSelector mechanics
03-node-affinity.yaml	❤️ Use requiredDuringSchedulingIgnoredDuringExecution for strict node affinity
04-node-anti-affinity.yaml	🚫 Avoid scheduling pods on certain nodes using node anti-affinity
05-pod-affinity.yaml	🤝 Co-locate pods for communication or proximity (e.g., cache + app)
06-pod-anti-affinity.yaml	⚖️ Distribute pods to avoid single-point failure (e.g., replicas across zones)
07-use-case.yaml	🧩 Combine multiple placement rules to reflect production-grade deployment
🚀 Quick Mnemonic
Here's a mnemonic to simplify these concepts: 🧠 N.A.P.S.U = NodeSelector, Affinity, PodSelector, Spread, Use-case

N = 🎯 nodeSelector — direct label match
A = ❤️ Affinity — prefer or require certain nodes
P = 🤝 PodAffinity — place pods together
S = ⚖️ PodAntiAffinity — separate replicas across nodes
U = 🧩 Use-case — real-world combination of strategies
🔗 When to Use What?
Strategy	When to Use
nodeSelector	When placement is simple and label-driven
nodeAffinity	For complex node conditions (preferred vs required)
podAffinity	Co-locating collaborating services (e.g., app ↔ cache)
podAntiAffinity	High availability with distributed replicas
