---
title: Тип ресурса mediaConfig
description: Конфигурация мультимедиа, используемый для подключения к звонку.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e4f6e940cd319d10cd3f03e3c94d0473164beb29
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515106"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="4aed7-103">Тип ресурса mediaConfig</span><span class="sxs-lookup"><span data-stu-id="4aed7-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4aed7-104">Конфигурация мультимедиа, используемый для подключения к звонку.</span><span class="sxs-lookup"><span data-stu-id="4aed7-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="4aed7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4aed7-105">Properties</span></span>

| <span data-ttu-id="4aed7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4aed7-106">Property</span></span>       | <span data-ttu-id="4aed7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4aed7-107">Type</span></span>    | <span data-ttu-id="4aed7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4aed7-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4aed7-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="4aed7-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="4aed7-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="4aed7-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="4aed7-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4aed7-111">JSON representation</span></span>

<span data-ttu-id="4aed7-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4aed7-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
  ],
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
