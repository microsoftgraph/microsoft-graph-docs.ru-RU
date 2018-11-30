---
title: educationOneRosterApiDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при использовании OneRoster API в качестве источника ввода.
ms.openlocfilehash: 0fd9c87c9934fc86d4e6788a5db42eb036fdb04f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078423"
---
# <a name="educationonerosterapidataprovider-resource"></a>educationOneRosterApiDataProvider ресурсов

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Используется для настройки синхронизации профилей данных school при использовании [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) в качестве источника ввода.

На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
|:-|:-|:-|
| **connectionUrl** | String | URL-адрес подключения к экземпляру OneRoster. |
| **schoolsIds** | Коллекция String |  Список sourcedIds school для синхронизации. |
| **providerName** | String | Имя поставщика услуг OneRoster, определенный в [спецификации OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA). |
| **connectionsettings используется для определения** | [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md) | Параметры подключения для экземпляра OneRoster. Должен иметь тип [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) или [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md). |
| **пользовательских настроек** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Дополнительные настройки применяется для синхронизации профилей.|

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
