---
title: Интеграция решений по обеспечению безопасности с помощью Microsoft Graph Security API
description: Используйте эти параметры для подключения к Microsoft Graph Security API и работы с данными в унифицированном формате от поддерживаемых Microsoft и партнерских поставщиков безопасности.
author: preetikr
ms.localizationpriority: high
ms.prod: security
ms.openlocfilehash: c221192e91d357c442dfd3eaa8ad32ae1685358e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437550"
---
# <a name="security-solution-integrations-using-the-microsoft-graph-security-api"></a>Интеграция решений по обеспечению безопасности с помощью Microsoft Graph Security API

К Microsoft Graph Security API можно подключиться с помощью следующих возможностей. Эти параметры позволяют работать с данными в унифицированном формате от [поддерживаемых Майкрософт и партнерских поставщиков безопасности](/graph/api/resources/security-api-overview#alerts) посредством единой интеграции:

- **Используйте поддерживаемые варианты интеграции:** обратитесь к [списку поддерживаемых вариантов интеграции](./security-concept-overview.md#why-use-the-microsoft-graph-security-api), таких как написание кода, чтобы напрямую подключить ваше приложение для получения ценных сведений. Используйте [примеры](https://aka.ms/graphsecurityapicode), чтобы приступить к работе.
- **Используйте встроенные интеграции и соединители, созданные партнерами Microsoft:** см. партнерские решения [Microsoft Graph Security API](https://aka.ms/graphsecuritypartnerships), чтобы использовать эти интеграции.  
- **Используйте соединители, созданные корпорацией Майкрософт:** см. [список соединителей](#list-of-connectors-from-microsoft), которые можно использовать для подключения к API с помощью различных решений для управления инцидентами безопасности (SIEM), реагированием и оркестровкой безопасности (SOAR), отслеживанием инцидентов и управлением услугами (ITSM). ), отчетности и так далее.  

## <a name="list-of-connectors-from-microsoft"></a>Список соединителей от Майкрософт

| Тип решения | Имя | Соединитель | Объявление |
|:-----|:--------|:--------|:----------|
| SIEM |Splunk Enterprise и Splunk Cloud|[Надстройка Microsoft Graph Security API для Splunk](https://aka.ms/graphsecuritysplunkaddon) | [Запись блога](https://aka.ms/graphsecuritysplunkaddonblogpost)<br>[Запись блога о Splunk в облаке](https://aka.ms/graphsecuritysplunkcloudblogpost)|
| SIEM |QRadar|[Протокол Microsoft Graph Security API и поддерживаемые QRadar DSM](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/com.ibm.dsm.doc/c_logsource_Microsoft_Graph_Security_protocol.html)| - |
| ITSM |ServiceNow|[Интеграция приема оповещений Microsoft Graph Security API](https://docs.servicenow.com/bundle/orlando-security-management/page/product/secops-integration-sir/secops-integration-ms-graph/concept/ms-graph-about.html)| - |
| SOAR | Azure Logic Apps / Microsoft Flow | [Соединитель Microsoft Graph Security для Azure Logic Apps, Microsoft Flow и Power Apps](/azure/connectors/connectors-integrate-security-operations-create-api-microsoft-graph-security) | [Запись блога](https://aka.ms/graphsecurityconnectorsblogpost) |
| Автоматизация | Модуль PowerShell | [Модуль PowerShell Microsoft Graph Security](https://aka.ms/graphsecuritypowershellmodule) | [Запись блога](https://aka.ms/graphsecuritypowershellmodulepost) |
| Отчетность | Power BI | [Соединитель Microsoft Graph Security для Power BI](/power-bi/connect-data/desktop-connect-graph-security) | [Запись блога](https://aka.ms/graphsecuritypowerbiconnectorblogpost) |

Если вы хотите поддерживать встроенную интеграцию в своем решении или стать поставщиком данных для Microsoft Graph Security API, ознакомьтесь [с возможностями партнерства](./security-partner-overview.md).
