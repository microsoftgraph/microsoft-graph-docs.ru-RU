---
title: ресурс educationOneRosterApiDataProvider
description: Используется для настройка профиля синхронизации школьных данных, когда API OneRoster используется в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2c90c7132f6e51b84e987cf6bda63baacc60b8ba
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080423"
---
# <a name="educationonerosterapidataprovider-resource"></a>ресурс educationOneRosterApiDataProvider

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для настройка профиля синхронизации школьных данных, когда [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) используется в качестве источника ввода.

Производный от [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство           | Тип                                         | Описание                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| connectionUrl      | String                                       | URL-адрес подключения к экземпляру OneRoster.                                                         |
| providerName       | String                                       | Имя поставщика услуг OneRoster, определенное спецификацией [OneRoster.][oneroster]           |
| schoolsIds         | Коллекция String                            | Список [синхронизируются с School/Org.][orgs] `sourcedId`                                                   |
| termIds            | Коллекция String                            | Список [академических сеансов для][terms] синхронизации.                                                       |
| connectionSettings | [educationSynchronizationConnectionSettings] | Параметры [OAuth 1.0][onerosteroauth1] или [OAuth 2.0][onerosteroauth2] для экземпляра OneRoster. |
| настройки     | [educationSynchronizationCustomizations]    | Необязательная настройка, которая будет применена к профилю синхронизации.                                  |

> [!IMPORTANT]
> OneRoster использует академические сеансы, а не один учебный год для сегментации данных. Эта сегментация абстрагироваться в Синхронизация сведений о школе пользовательского интерфейса, но не этот API. Чтобы заполнить коллекцию, необходимо вызвать конечную точку OneRoster, чтобы получить коллекцию академических ИД `/terms` `termIds` сеансов.

[educationSynchronizationConnectionSettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md
[oneroster]: https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA
[onerosteroauth2]: educationsynchronizationoauth2clientcredentialsconnectionsettings.md
[onerosteroauth1]: educationsynchronizationoauth1connectionsettings.md
[terms]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452034
[orgs]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452016

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type&quot;: &quot;microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
  "connectionUrl": "String",
  "providerName": "String",
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings",
    "clientId": "String",
    "clientSecret&quot;: &quot;String"
  },
  "customizations": {
    "@odata.type&quot;: &quot;microsoft.graph.educationSynchronizationCustomizations"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneRosterApiDataProvider resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.ediscovery.settings"
  ]
}-->


