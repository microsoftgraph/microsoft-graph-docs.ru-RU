---
title: Интеграция решений по обеспечению безопасности с помощью Microsoft Graph Security API
description: Все возможности, описанные в этой статье, позволяют подключаться к Microsoft Graph Security API. Эти возможности позволяют работать с данными в едином формате в разных поддерживаемых решениях поставщиков безопасности партнеров и Майкрософт с помощью единой интеграции.
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: e3c4aa756de62995deef07604d968b172ffc2645
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038515"
---
# <a name="security-solution-integrations-using-the-microsoft-graph-security-api"></a>Интеграция решений по обеспечению безопасности с помощью Microsoft Graph Security API

К Microsoft Graph Security API можно подключиться с помощью следующих возможностей. Они позволяют работать с данными в едином формате в разных [поддерживаемых решениях поставщиков безопасности партнеров и Майкрософт](https://aka.ms/graphsecurityalerts) с помощью единой интеграции.

- **Непосредственное использование поддерживаемых вариантов интеграции**. См. [список поддерживаемых вариантов интеграции](https://docs.microsoft.com/graph/security-concept-overview#why-use-the-microsoft-graph-security-api), например написание кода для прямого подключения приложения, чтобы получать более подробные сведения. Используйте [примеры](https://aka.ms/graphsecurityapicode), чтобы приступить к работе.
- **Использование встроенной интеграции и соединителей, созданных партнерами Майкрософт**. Чтобы использовать эти возможности интеграции, ознакомьтесь с [решениями партнеров для Microsoft Graph Security API](https://aka.ms/graphsecuritypartnerships).  
- **Использование соединителей, созданных Майкрософт**. См. [список соединителей](https://aka.ms/graphsecuritysolutionsconnectors), которые можно использовать для подключения к API с помощью разных решений для служб SIEM (инциденты безопасности и управление), SOAR (реагирование системы безопасности и согласование), ITSM (отслеживание инцидентов и управление службой), отчетности и т. д.  

## <a name="list-of-connectors-from-microsoft"></a>Список соединителей от Майкрософт

| Тип решения | Имя | Соединитель | Объявление |
|:-----|:--------|:--------|:----------|
| SIEM |Splunk Enterprise и Splunk Cloud|[Надстройка Microsoft Graph Security API для Splunk](https://aka.ms/graphsecuritysplunkaddon) | [Запись блога](https://aka.ms/graphsecuritysplunkaddonblogpost)<br>[Запись блога о Splunk в облаке](https://aka.ms/graphsecuritysplunkcloudblogpost)|
| SIEM |QRadar|[Протокол Microsoft Graph Security API и поддерживаемые QRadar DSM](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/com.ibm.dsm.doc/c_logsource_Microsoft_Graph_Security_protocol.html)| - |
| ITSM |ServiceNow|[Интеграция приема оповещений Microsoft Graph Security API](https://docs.servicenow.com/bundle/orlando-security-management/page/product/secops-integration-sir/secops-integration-ms-graph/concept/ms-graph-about.html)| - |
| SOAR | Azure Logic Apps / Microsoft Flow | [Соединитель Microsoft Graph Security для Azure Logic Apps, Microsoft Flow и PowerApps](https://aka.ms/graphsecurityconnectors) | [Запись блога](https://aka.ms/graphsecurityconnectorsblogpost) |
| Автоматизация | Модуль PowerShell | [Модуль PowerShell Microsoft Graph Security](https://aka.ms/graphsecuritypowershellmodule) | [Запись блога](https://aka.ms/graphsecuritypowershellmodulepost) |
| Отчетность | Power BI | [Соединитель Microsoft Graph Security для Power BI](https://aka.ms/graphsecuritypowerbiconnectordoc) | [Запись блога](https://aka.ms/graphsecuritypowerbiconnectorblogpost) |

Ознакомьтесь с [возможностями партнерства](https://docs.microsoft.com/graph/security-partner-overview), если вы хотите поддерживать встроенную интеграцию в своем решении или стать поставщиком данных для Microsoft Graph Security API.
