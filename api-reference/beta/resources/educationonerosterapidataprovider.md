---
title: ресурс Едукатиононеростерапидатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании API OneRoster в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b96322cdb408069136a46aa9c83cf363cc1b6f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998847"
---
# <a name="educationonerosterapidataprovider-resource"></a>ресурс Едукатиононеростерапидатапровидер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для настройки профиля синхронизации данных School при использовании [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) в качестве источника входных данных.

Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство           | Тип                                         | Описание                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| коннектионурл      | String                                       | URL-адрес подключения к экземпляру OneRoster.                                                         |
| providerName       | String                                       | Имя поставщика службы OneRoster, как определено [спецификацией OneRoster][oneroster].           |
| счулсидс         | Коллекция String                            | Список учебных заведений [или организации][orgs] `sourcedId` для синхронизации.                                                   |
| термидс            | Коллекция String                            | Список [учебных лекций][terms] для синхронизации.                                                       |
| коннектионсеттингс | [едукатионсинчронизатионконнектионсеттингс] | Параметры [oauth 1,0][onerosteroauth1] или [OAuth 2,0][onerosteroauth2] для экземпляра OneRoster. |
| настроек     | [едукатионсинчронизатионкустомизатионс])    | Необязательная настройка, применяемая к профилю синхронизации.                                  |

> [!IMPORTANT]
> В OneRoster для сегментирования данных используются учебные сеансы, а не один учебный год. Эта сегментация абстрактна в пользовательском интерфейсе "School Data Sync", но не является этим API. Для заполнения коллекции необходимо вызвать `/terms` конечную точку OneRoster для получения коллекции академических идентификаторов сеансов `termIds` .

[едукатионсинчронизатионконнектионсеттингс]: educationsynchronizationconnectionsettings.md
[едукатионсинчронизатионкустомизатионс]: educationsynchronizationcustomizations.md
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
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
  "connectionUrl": "String",
  "providerName": "String",
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
  },
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
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
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.settings"
  ]
}-->


