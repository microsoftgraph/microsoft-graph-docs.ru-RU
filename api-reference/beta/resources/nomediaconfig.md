---
title: Тип ресурса Номедиаконфиг
description: Конфигурация мультимедиа, указывающая на отсутствие носителя.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8d564493889cc367ecdb697ce4031c40a4cbbbef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581640"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="ce790-103">Тип ресурса Номедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="ce790-103">noMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce790-104">Конфигурация мультимедиа, указывающая на отсутствие носителя.</span><span class="sxs-lookup"><span data-stu-id="ce790-104">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="ce790-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce790-105">Properties</span></span>

| <span data-ttu-id="ce790-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce790-106">Property</span></span>       | <span data-ttu-id="ce790-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ce790-107">Type</span></span>    | <span data-ttu-id="ce790-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ce790-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ce790-109">Ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="ce790-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="ce790-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce790-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="ce790-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce790-111">JSON representation</span></span>

<span data-ttu-id="ce790-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce790-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
