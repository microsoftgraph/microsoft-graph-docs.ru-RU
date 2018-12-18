---
title: Интеграция оповещений API безопасности Microsoft Graph с SIEM
description: API безопасности Microsoft Graph позволяет управлять предупреждениями системы безопасности всех продуктов безопасности корпорации Майкрософт, известными как поставщики услуг безопасности Microsoft Graph, через единую конечную точку REST. В некоторых организациях в решения SIEM через Azure Monitor уже могут приниматься данные журналов, относящиеся к Azure. Для упрощения интеграции предупреждения системы безопасности, доступные в API безопасности Microsoft Graph, могут быть также использоваться клиентом в его подписке через Azure Monitor. Если в вашей организации уже настроена интеграция Azure Monitor с решением SIEM, то вы можете с легкостью выполнять потоковую передачу оповещений системы безопасности вашей организации в дополнение к существующим данным, доступным через Azure Monitor.
author: Preetikr
ms.openlocfilehash: 24b2261e2a320e5384fba97802eab43991c34254
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327386"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Интеграция оповещений API безопасности Microsoft Graph с SIEM

API безопасности Microsoft Graph позволяет управлять предупреждениями системы безопасности всех продуктов безопасности корпорации Майкрософт, известными как поставщики услуг безопасности Microsoft Graph, через единую конечную точку REST. В некоторых организациях в решения SIEM через Azure Monitor уже могут приниматься данные журналов, относящиеся к Azure. Для упрощения интеграции предупреждения системы безопасности, доступные в API безопасности Microsoft Graph, могут быть также использоваться клиентом в его подписке через Azure Monitor. Если в вашей организации уже настроена интеграция Azure Monitor с решением SIEM, то вы можете с легкостью выполнять потоковую передачу оповещений системы безопасности вашей организации в дополнение к существующим данным, доступным через Azure Monitor.

Azure Monitor поддерживает соединители для нескольких продуктов SIEM. Список поддерживаемых SIEM продуктов см. в статье [отправка данных наблюдения в Центр отправки](https://docs.microsoft.com/ru-RU/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Интеграция API безопасности Microsoft Graph доступна для [Splunk](https://splunkbase.splunk.com/) и [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem).

Дополнительные сведения об интеграции API безопасности Microsoft Graph для определенных решений SIEM:

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
