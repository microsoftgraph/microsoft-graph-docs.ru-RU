---
title: Тип ресурса commsNotifications
description: Список уведомлений, используемого серверами коммуникаций для отправки нескольких уведомлений в одном пакете.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2d002b74bffe0911e2ba1fef4eed324b52ebcc49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520594"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="5c3b3-103">Тип ресурса commsNotifications</span><span class="sxs-lookup"><span data-stu-id="5c3b3-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c3b3-104">Список уведомлений, используемого серверами коммуникаций для отправки нескольких уведомлений в одном пакете.</span><span class="sxs-lookup"><span data-stu-id="5c3b3-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="5c3b3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c3b3-105">Properties</span></span>

| <span data-ttu-id="5c3b3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c3b3-106">Property</span></span>       | <span data-ttu-id="5c3b3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5c3b3-107">Type</span></span>                                                 | <span data-ttu-id="5c3b3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5c3b3-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="5c3b3-109">value</span><span class="sxs-lookup"><span data-stu-id="5c3b3-109">value</span></span>          | <span data-ttu-id="5c3b3-110">[commsNotification](commsnotification.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5c3b3-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="5c3b3-111">Уведомление об изменении в ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5c3b3-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5c3b3-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c3b3-112">JSON representation</span></span>

<span data-ttu-id="5c3b3-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c3b3-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/commsnotifications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
