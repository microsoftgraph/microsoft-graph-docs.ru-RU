---
title: ресурс Едукатиононеростерапидатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании API OneRoster в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca94043fdf215d47a1ccaf16f3a667f1178c1d57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972637"
---
# <a name="educationonerosterapidataprovider-resource"></a>ресурс Едукатиононеростерапидатапровидер

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для настройки профиля синхронизации данных School при использовании [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) в качестве источника входных данных.

Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Коннектионурл** | String | URL-адрес подключения к экземпляру OneRoster. |
| **Счулсидс** | Коллекция строк |  Список Саурцедидс School для синхронизации. |
| **providerName** | String | Имя поставщика службы OneRoster, как определено [спецификацией OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA). |
| **Коннектионсеттингс** | [Microsoft. Graph. Едукатионсинчронизатионконнектионсеттингс](educationsynchronizationconnectionsettings.md) | Параметры подключения для экземпляра OneRoster. Должен иметь тип [Microsoft. Graph. educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) или [Microsoft. Graph. educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md). |
| **настроек** | [Microsoft. Graph. Едукатионсинчронизатионкустомизатионс](educationsynchronizationcustomizations.md) | Необязательная настройка, применяемая к профилю синхронизации.|

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
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
