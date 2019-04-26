---
title: Интеграция оповещений API безопасности Microsoft Graph с SIEM
description: API безопасности Microsoft Graph позволяет управлять предупреждениями системы безопасности всех продуктов безопасности корпорации Майкрософт, известными как поставщики услуг безопасности Microsoft Graph, через единую конечную точку REST. В некоторых организациях в решения SIEM через Azure Monitor уже могут приниматься данные журналов, относящиеся к Azure. Для упрощения интеграции предупреждения системы безопасности, доступные в API безопасности Microsoft Graph, могут быть также использоваться клиентом в его подписке через Azure Monitor. Если в вашей организации уже настроена интеграция Azure Monitor с решением SIEM, то вы можете с легкостью выполнять потоковую передачу оповещений системы безопасности вашей организации в дополнение к существующим данным, доступным через Azure Monitor.
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 92a5416f68ccbc6fbbd0001c473f1daf2fe21187
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556932"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Интеграция оповещений API безопасности Microsoft Graph с SIEM

API безопасности Microsoft Graph позволяет управлять предупреждениями системы безопасности всех продуктов безопасности корпорации Майкрософт, известными как поставщики услуг безопасности Microsoft Graph, через единую конечную точку REST. В некоторых организациях в решения SIEM через Azure Monitor уже могут приниматься данные журналов, относящиеся к Azure. Для упрощения интеграции предупреждения системы безопасности, доступные в API безопасности Microsoft Graph, могут быть также использоваться клиентом в его подписке через Azure Monitor. Если в вашей организации уже настроена интеграция Azure Monitor с решением SIEM, то вы можете с легкостью выполнять потоковую передачу оповещений системы безопасности вашей организации в дополнение к существующим данным, доступным через Azure Monitor.

При использовании интеграции с SIEM доступны оповещения от указанных ниже поставщиков безопасности.

- [Центр безопасности Azure](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Защита идентификации Azure Active Directory](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts)
- [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(предварительная версия)**
- [Расширенная защита от угроз Azure](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories) **(предварительная версия)**
- [Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility) **(предварительная версия)**

Azure Monitor поддерживает соединители для нескольких продуктов SIEM. Список поддерживаемых SIEM продуктов см. в статье [отправка данных наблюдения в Центр отправки](https://docs.microsoft.com/ru-RU/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Интеграция API безопасности Microsoft Graph доступна для [Splunk](https://splunkbase.splunk.com/) и [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem).

Дополнительные сведения об интеграции API безопасности Microsoft Graph для определенных решений SIEM:

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
