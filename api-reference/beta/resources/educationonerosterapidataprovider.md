---
title: ресурс Едукатиононеростерапидатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании API OneRoster в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 55a3cd0e20f15c4b7d44bc7aebdc19f202e044f1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543000"
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
| **providerName** | String | Имя поставщика службы OneRoster, как определено [спецификациЕй OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA). |
| **Коннектионсеттингс** | [Microsoft. Graph. Едукатионсинчронизатионконнектионсеттингс](educationsynchronizationconnectionsettings.md) | Параметры подключения для экземпляра OneRoster. Должен иметь тип [Microsoft. Graph. educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) или [Microsoft. Graph. educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md). |
| **настроек** | [Microsoft. Graph. Едукатионсинчронизатионкустомизатионс](educationsynchronizationcustomizations.md) | НеОбязательная Настройка, применяемая к профилю синхронизации.|

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonerosterapidataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
