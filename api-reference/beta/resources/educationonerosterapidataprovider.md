---
title: educationOneRosterApiDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при использовании OneRoster API в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 681a3331aba7bc84ac80911c4be8076d104f8a58
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938148"
---
# <a name="educationonerosterapidataprovider-resource"></a>educationOneRosterApiDataProvider ресурсов

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Используется для настройки синхронизации профилей данных school при использовании [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) в качестве источника ввода.

На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **connectionUrl** | Строка | URL-адрес подключения к экземпляру OneRoster. |
| **schoolsIds** | Коллекция String |  Список sourcedIds school для синхронизации. |
| **providerName** | Строка | Имя поставщика услуг OneRoster, определенный в [спецификации OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA). |
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
