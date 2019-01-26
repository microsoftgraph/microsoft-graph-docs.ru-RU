---
title: Тип ресурса serviceHostedMediaConfig
description: Тип serviceHostedMediaConfig.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 127450b569a37f00a76696a749c269f55c15b7aa
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572453"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="cb054-103">Тип ресурса serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="cb054-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb054-104">Тип serviceHostedMediaConfig.</span><span class="sxs-lookup"><span data-stu-id="cb054-104">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="cb054-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb054-105">Properties</span></span>

| <span data-ttu-id="cb054-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb054-106">Property</span></span>                    | <span data-ttu-id="cb054-107">Тип</span><span class="sxs-lookup"><span data-stu-id="cb054-107">Type</span></span>                                                        | <span data-ttu-id="cb054-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cb054-108">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="cb054-109">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="cb054-109">preFetchMedia</span></span>               | <span data-ttu-id="cb054-110">[mediaInfo](mediainfo.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cb054-110">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="cb054-111">Список мультимедиа для предварительно выборки.</span><span class="sxs-lookup"><span data-stu-id="cb054-111">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="cb054-112">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="cb054-112">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="cb054-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb054-113">Boolean</span></span>                                                     | <span data-ttu-id="cb054-114">Удалите собственный участника из группы по умолчанию звука.</span><span class="sxs-lookup"><span data-stu-id="cb054-114">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cb054-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb054-115">JSON representation</span></span>

<span data-ttu-id="cb054-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb054-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
   "baseType":"microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a><span data-ttu-id="cb054-117">Пример</span><span class="sxs-lookup"><span data-stu-id="cb054-117">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [
    {
      "uri": "https://cdn.contoso.com/beep.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
    },
    {
      "uri": "https://cdn.contoso.com/cool.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
    }
  ],
  "removeFromDefaultAudioGroup": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/servicehostedmediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
