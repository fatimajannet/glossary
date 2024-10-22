---
title: Инфраструктура как код (IaC)
status: Completed
category: concept
tags: ["infrastructure", "methodology", ""]
---

Инфраструктура как код (Infrastructure as Code) — подход, при котором описание инфраструктуры хранится в виде одного или нескольких файлов. 
Этот подход пришел на смену традиционной модели, в которой инфраструктура как услуга (Infrastructure as a Service) предоставляется вручную, 
обычно с помощью shell-скриптов или других инструментов конфигурирования.

## Какую проблему решает

Подход к разработке нативных облачных приложений требует, чтобы инфраструктура была одноразовой и воспроизводимой. 
Также она должна [масштабироваться](/scalability/) по запросу автоматизированным и воспроизводимым образом, желательно без вмешательства человека. 
Ручное управление инфраструктурой не удовлетворяет требованиям к скорости и масштабированию, которые предъявляются к [нативным облачным приложениям](/ru/cloud-native-apps/). 
Изменения инфраструктуры, сделанные вручную, не обладают воспроизводимостью, кроме того, они плохо масштабируются и приводят к ошибкам в конфигурации.

## Как именно решает проблему

Представляя ресурсы дата-центра (серверы, балансировщики нагрузки, подсети и т. п.) в виде кода, 
инфраструктурные команды получают единый источник истины для всех конфигураций и возможность 
управлять центром обработки данных с помощью пайплайнов [CI](/ru/continuous-integration/)/[CD](/ru/continuous-delivery/), 
используя при этом контроль версий и стратегии развертывания.