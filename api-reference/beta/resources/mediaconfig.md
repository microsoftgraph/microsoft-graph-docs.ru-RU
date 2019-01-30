---
title: Тип ресурса mediaConfig
description: Конфигурация мультимедиа, используемый для подключения к звонку.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e4f6e940cd319d10cd3f03e3c94d0473164beb29
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642620"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="b3be9-103">Тип ресурса mediaConfig</span><span class="sxs-lookup"><span data-stu-id="b3be9-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3be9-104">Конфигурация мультимедиа, используемый для подключения к звонку.</span><span class="sxs-lookup"><span data-stu-id="b3be9-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="b3be9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3be9-105">Properties</span></span>

| <span data-ttu-id="b3be9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3be9-106">Property</span></span>       | <span data-ttu-id="b3be9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b3be9-107">Type</span></span>    | <span data-ttu-id="b3be9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b3be9-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b3be9-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="b3be9-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="b3be9-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3be9-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="b3be9-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3be9-111">JSON representation</span></span>

<span data-ttu-id="b3be9-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3be9-112">The following is a JSON representation of the resource.</span></span>

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
