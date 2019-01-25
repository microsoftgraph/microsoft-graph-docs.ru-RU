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
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="d38f4-103">educationSynchronizationOAuth1ConnectionSettings ресурсов</span><span class="sxs-lookup"><span data-stu-id="d38f4-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d38f4-104">При OAuth1 будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="d38f4-104">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="d38f4-105">На основе [microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="d38f4-105">Derived from [microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d38f4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d38f4-106">Properties</span></span>

<span data-ttu-id="d38f4-107">Дополнительные свойства, предоставляемые интерфейсом этого типа.</span><span class="sxs-lookup"><span data-stu-id="d38f4-107">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d38f4-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d38f4-108">JSON representation</span></span>
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
