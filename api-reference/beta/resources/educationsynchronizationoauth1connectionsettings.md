---
title: educationSynchronizationOAuth1ConnectionSettings ресурсов
description: При OAuth1 будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 71e45033c022061b72c1ea0be815ff3e0b611475
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516674"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a>educationSynchronizationOAuth1ConnectionSettings ресурсов

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

При OAuth1 будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.

На основе [microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).

## <a name="properties"></a>Свойства

Дополнительные свойства, предоставляемые интерфейсом этого типа.

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationoauth1connectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
