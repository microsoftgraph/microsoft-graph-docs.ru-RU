---
title: Тип ресурса Коммснотификатионс
description: Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2d002b74bffe0911e2ba1fef4eed324b52ebcc49
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535524"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="da9fe-103">Тип ресурса Коммснотификатионс</span><span class="sxs-lookup"><span data-stu-id="da9fe-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da9fe-104">Список уведомлений, используемых серверами Communications Server для отправки нескольких уведомлений в один пакет.</span><span class="sxs-lookup"><span data-stu-id="da9fe-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="da9fe-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="da9fe-105">Properties</span></span>

| <span data-ttu-id="da9fe-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="da9fe-106">Property</span></span>       | <span data-ttu-id="da9fe-107">Тип</span><span class="sxs-lookup"><span data-stu-id="da9fe-107">Type</span></span>                                                 | <span data-ttu-id="da9fe-108">Описание</span><span class="sxs-lookup"><span data-stu-id="da9fe-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="da9fe-109">значение</span><span class="sxs-lookup"><span data-stu-id="da9fe-109">value</span></span>          | <span data-ttu-id="da9fe-110">Коллекция [коммснотификатион](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="da9fe-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="da9fe-111">Уведомление об изменении ресурса.</span><span class="sxs-lookup"><span data-stu-id="da9fe-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da9fe-112">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="da9fe-112">JSON representation</span></span>

<span data-ttu-id="da9fe-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da9fe-113">The following is a JSON representation of the resource.</span></span>

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
