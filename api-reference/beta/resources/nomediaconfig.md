---
title: Тип ресурса noMediaConfig
description: Конфигурация мультимедиа, указывающие нет носителя.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 06ca7f2c49c23575487d95bdb555d03d86860849
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573573"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="698a2-103">Тип ресурса noMediaConfig</span><span class="sxs-lookup"><span data-stu-id="698a2-103">noMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="698a2-104">Конфигурация мультимедиа, указывающие нет носителя.</span><span class="sxs-lookup"><span data-stu-id="698a2-104">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="698a2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="698a2-105">Properties</span></span>

| <span data-ttu-id="698a2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="698a2-106">Property</span></span>       | <span data-ttu-id="698a2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="698a2-107">Type</span></span>    | <span data-ttu-id="698a2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="698a2-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="698a2-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="698a2-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="698a2-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="698a2-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="698a2-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="698a2-111">JSON representation</span></span>

<span data-ttu-id="698a2-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="698a2-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.noMediaConfig"
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
  "description": "noMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/nomediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
